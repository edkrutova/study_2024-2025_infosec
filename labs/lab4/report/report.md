---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Дискреционное разграничение прав в Linux. Расширенные атрибуты"
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

Целью данной работы является приобретение практических навыков работы в консоли с расширенными атрибутами файлов.

# Выполнение лабораторной работы

1. Выполнение пунктов (рис. [-@fig:001] - [-@fig:0011]).

![Просмотр расширенных атрибутов файла file1](image/Screenshot_1.png){#fig:001 width=70%}

![Установка прав на файл file1, разрешающих чтение и запись для владельца файла](image/Screenshot_2.png){#fig:002 width=70%}

![Попытка установить на файл file1 расширенный атрибут a](image/Screenshot_3.png){#fig:003 width=70%}

![Установка на файл file1 расширенный атрибут a с консоли с правами администраторв](image/Screenshot_4.png){#fig:004 width=70%}

![Просмотр расширенных атрибутов файла file1](image/Screenshot_5.png){#fig:005 width=70%}

![Дозапись в файл file1 слова «test»](image/Screenshot_6.png){#fig:006 width=70%}

![Попытка стереть имеющуюся в файле file1 информацию](image/Screenshot_7.png){#fig:007 width=70%}

![Попытка переименовать файл](image/Screenshot_8.png){#fig:008 width=70%}

![Попытка установить на файл file1 иные права](image/Screenshot_9.png){#fig:009 width=70%}

![Удаление атрибута a](image/Screenshot_10.png){#fig:010 width=70%}

![Переименование файла и изменение прав](image/Screenshot_11.png){#fig:011 width=70%}

После удаления атрибута a с файлом стали доступные разрешённые правами доступа действия.

# Выводы

Я приобрела практические навыки работы в консоли с расширенными атрибутами файлов.
