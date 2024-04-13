---
## Front matter
title: "Отчёт по лабораторной работе №10"
subtitle: "Операционные системы"
author: "Бережной Иван Александрович"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 13pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание

1. Создание нового файла с использованием vi
2. Редактирование существующего файла

# Теоретическое введение

В большинстве дистрибутивов Linux в качестве текстового редактора по умолчанию устанавливается интерактивный экранный редактор vi (Visual display editor).
Редактор vi имеет три режима работы:
– командный режим — предназначен для ввода команд редактирования и навигации по редактируемому файлу;
– режим вставки — предназначен для ввода содержания редактируемого файла;
– режим последней (или командной) строки — используется для записи изменений в файл и выхода из редактора.
Для вызова редактора vi необходимо указать команду vi и имя редактируемого файла: vi <имя_файла>
При этом в случае отсутствия файла с указанным именем будет создан такой файл.
Переход в командный режим осуществляется нажатием клавиши Esc . Для выхода из редактора vi необходимо перейти в режим последней строки: находясь в командном режиме, нажать Shift-; (по сути символ : — двоеточие), затем:
– набрать символы wq, если перед выходом из редактора требуется записать изменения в файл;
– набрать символ q (или q!), если требуется выйти из редактора без сохранения.

# Выполнение лабораторной работы

## Создание нового файла с использованием vi
Сначала создадим каталог, в котором будем сегодня работать и перейдём в него. Вызовем vi, попутно создав новый файл (рис. [-@fig:001]).

![Вызов vi](image/1.jpg){#fig:001 width=70%}

Нажимаем "i" и вводим текст из предложенного листинга (рис. [-@fig:002]).

![Ввод текста](image/2.jpg){#fig:002 width=70%}

Переходим в командный режим, затем в режим последней строки и пишем "wq" внизу экрана, чтобы записать текст и выйти из vi (рис. [-@fig:003]).

![Режим последней строки](image/3.jpg){#fig:003 width=70%}

Сделаем файл исполняемым с помощью команды chmod (рис. [-@fig:004]).

![Изменение прав доступа](image/4.jpg){#fig:004 width=70%}

## Редактирование существующего файла
Установим курсор в конце слова HELL второй строки, перейдём в режим вставки и заменим слово на HELLO, затем заменим слово LOCAL на local и в конце файла напишем `echo $HELLO` (рис. [-@fig:005]).
Теперь удалим последнюю строку (рис. [-@fig:006]), затем отменим это действие командой "u" в командном режиме (рис. [-@fig:007]).
Запишем эти изменения в режиме последней строки и выйдем из vi.

![Изменение файла](image/5.jpg){#fig:005 width=70%}

![Удаление строки](image/6.jpg){#fig:006 width=70%}

![Возврат действия](image/5.jpg){#fig:007 width=70%}

# Выводы

В ходе выполнения лабораторной работы мы познакомились с операционной системой Linux и получили практические навыки работы с редактором vi.

# Список литературы{.unnumbered}
