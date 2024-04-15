---
## Front matter
title: "Отчёт по третьему этапу индивидуального проекта"
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

Научиться писать про свои навыки и достижения.

# Задание

1. Добавить информацию о навыках, опыте и достижениях
2. Сделать пост по прошедшей неделе
3. Добавить пост на тему "Язык разметки Markdown"

# Выполнение лабораторной работы

## Добавление информации о навыках, опыте и достижениях
Первым делом добавим информацию о своих навыках (рис. [-@fig:001]). Посмотрим, как это отображается на сайте (рис. [-@fig:002]).

![Описание навыков](image/1.jpg){#fig:001 width=70%}

![Отображение навыков](image/2.jpg){#fig:002 width=70%}

Теперь напишем про свой опыт. У меня его немного, а если точнее, я просто студент. Об этом и напишем (рис. [-@fig:003]). Также проверим, как это смотрится на сайте (рис. [-@fig:004]).

![Описание опыта](image/3.jpg){#fig:003 width=70%}

![Отображение опыта](image/4.jpg){#fig:004 width=70%}

Не забудем также указать свои достижения (рис. [-@fig:005]). Я написал про одно, а именно сертификат платформы Stepik по Питону (рис. [-@fig:006]).

![Описание достижений](image/5.jpg){#fig:005 width=70%}

![Отображение достижений](image/6.jpg){#fig:006 width=70%}

## Создание поста по прошедшей неделе
Напишем пост о том, как прошла моя предыдущая неделя. Она была совсем не насыщенная, поэтому писать было не о чем (рис. [-@fig:007]).

![Написание поста о прошедшей неделе](image/7.jpg){#fig:007 width=70%}

## Добавить пост на тему "Язык разметки Markdown"
И, наконец, напишем пост о Markdown. Информации очень много, поэтому я разделил её на несколько постов. Остальные будут выложены позднее (рис. [-@fig:008]). Посмотрим, как отображаются посты на сайте (рис. [-@fig:009]), а также, видно ли их в "Недавних постах" (рис. [-@fig:010]).

![Написание поста про Markdown](image/8.jpg){#fig:008 width=70%}

![Отображение поста](image/9.jpg){#fig:009 width=70%}

![Недавние посты](image/10.jpg){#fig:010 width=70%}

# Выводы

В ходе выполнения задания мы научились рассказывать о своих навыках, опыте и достижениях, а также потренировались выкладывать посты на разные темы.
