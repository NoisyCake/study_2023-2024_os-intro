---
## Front matter
title: "Отчёт по пятому этапу индивидуального проекта"
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

Добавить всю оставшуюся информацию о себе

# Задание

1. Добавить информацию
2. Сделать пост по прошедшей неделе
3. Сделать пост на тему "Языки научного программирования"

# Выполнение лабораторной работы

## Добавление ссылок
Для начала изменим раздел "Contact", где напишем нужный адрес, почту и телефон, вобьём новые координаты и на всякий случай включим капчу при попытке отправить email (рис. [-@fig:001]). Также удалим неактуальные для студента блоки. Готово.

![Редактирование "Contact"](image/1.jpg){#fig:001 width=70%}

## Создание поста по прошедшей неделе
Сделаем пост по прошедшей неделе, описав самые интересные события из неё (рис. [-@fig:002]).

![Написание первого поста](image/2.jpg){#fig:002 width=70%}

## Создание тематического поста
Теперь напишем пост о том, как какие существуют научные языки программирования (рис. [-@fig:003]). Посмотрим, как это выглядит в "Постах" (рис. [-@fig:004]).

![Написание второго поста](image/3.jpg){#fig:003 width=70%}

![Просмотр поста](image/4.jpg){#fig:004 width=70%}

# Выводы

В ходе выполнения задания мы дополнили сайт информацией о себе.
