---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап 2"
author: "Крутова Екатерина Дмитриевна"

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
fontsize: 12pt
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

Целью данной работы является установка DVWA в гостевую систему к Kali Linux.

# Выполнение лабораторной работы

Установка DVWA в гостевую систему к Kali Linux (рис. [-@fig:001] - [-@fig:006]).

![Скачивание DVWA из репозитория](image/Screenshot_1.png){#fig:001 width=70%}

![Установка DVWA с помощью команды](image/Screenshot_2.png){#fig:002 width=70%}

![Завершение установки](image/Screenshot_3.png){#fig:003 width=70%}

![Скачивание необходимых пакетов](image/Screenshot_4.png){#fig:004 width=70%}

![Вход в DVWA](image/Screenshot_5.png){#fig:005 width=70%}

![Создание базы данных](image/Screenshot_6.png){#fig:006 width=70%}

![Завершение установки](image/Screenshot_7.png){#fig:007 width=70%}


# Выводы

Я установила DVWA в гостевую систему к Kali Linux.

# Список литературы
