---
## Front matter
title: "Отчёт по лабораторной работе №14"
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

Изучить основы программирования в оболочке ОС UNIX. Научиться писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

# Задание

1. Написать командный файл, реализующий упрощённый механизм семафоров
2. Реализовать команду man с помощью командного файла
3. Написать командный файл, генерирующий случайную последовательность букв латинского алфавита

# Выполнение лабораторной работы

## Написание первого командного файла
Создадим файл в терминале и присвоим ему право на исполнение. Напишем скрипт, который в течение некоторого времени дожидается освобождения ресурса, выдавая об этом сообщение, а дождавшись его освобождения, использует его в течение некоторого времени, также выдавая информацию о том, что ресурс используется соответствующим командным файлом (рис. [-@fig:001]). Запустим скрипт и проверим результат (рис. [-@fig:002]).

![Первый скрипт](image/1.jpg){#fig:001 width=70%}

![Запуск первого скрипта](image/2.jpg){#fig:002 width=70%}

## Написание второго командного файла
Создадим второй командный файл и также дадим ему право на исполнение. Реализуем команду man скриптом, который будет получать в виде аргумента командной строки название команды и в виде результата выдавать справку об этой команде или сообщение об отсутствии справки (рис. [-@fig:003]). Запустим файл (рис. [-@fig:004]) и получим такой результат (рис. [-@fig:005]).

![Второй скрипт](image/3.jpg){#fig:003 width=70%}

![Запуск второго скрипта](image/4.jpg){#fig:004 width=70%}

![Проверка работы скрипта](image/5.jpg){#fig:005 width=70%}

## Написание третьего командного файла
Теперь напишем командный файл, генерирующий случайную последовательность букв латинского алфавита (рис. [-@fig:006]). Запустим файл (рис. [-@fig:007])

![Третий скрипт](image/6.jpg){#fig:006 width=70%}

![Запуск третьего скрипта](image/7.jpg){#fig:007 width=70%}

# Выводы

В ходе выполнения лабораторной работы мы изучили основы программирования в оболочке ОС UNIX и научились писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

# Список литературы{.unnumbered}
