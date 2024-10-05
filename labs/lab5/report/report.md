---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Дискреционное разграничение прав в Linux. Исследование влияния дополнительных атрибутов"
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

Целью данной работы является изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов, получение практических навыков работы в консоли с дополнительными атрибутами, рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

# Выполнение лабораторной работы

1. Создание программы (рис. [-@fig:001] - [-@fig:018]).

![Вход в систему от имени пользователя guest](image/Screenshot_1.png){#fig:001 width=70%}

![Создание программы simpleid.c](image/Screenshot_2.png){#fig:002 width=70%}

![simpleid.c](image/Screenshot_3.png){#fig:003 width=70%}

![Компиляция программы simpleid.c](image/Screenshot_4.png){#fig:004 width=70%}

![Выполнение программы simpleid.c](image/Screenshot_5.png){#fig:005 width=70%}

![Выполнение системной программы id](image/Screenshot_6.png){#fig:006 width=70%}

Вывод идентичен.

![simpleid2.c](image/Screenshot_7.png){#fig:007 width=70%}

![Компиляция и выполнение](image/Screenshot_8.png){#fig:008 width=70%}

![Выполнение команд по изминению владельца файла и  установке SetU’D-бита](image/Screenshot_9.png){#fig:009 width=70%}

![Проверка установки атрибутов](image/Screenshot_10.png){#fig:010 width=70%}

![Выполнение  simpleid2 и id](image/Screenshot_11.png){#fig:011 width=70%}

![readfile.c](image/Screenshot_12.png){#fig:012 width=70%}

![Компиляция](image/Screenshot_13.png){#fig:013 width=70%}

![Изменение владельца и прав](image/Screenshot_14.png){#fig:014 width=70%}

![Попытка прочитать файл readfile.c](image/Screenshot_15.png){#fig:015 width=70%}

![Изменение владельца и установка SetU’D-бита](image/Screenshot_16.png){#fig:016 width=70%}

![Попытка прочитать файл readfile.c (неуспешно)](image/Screenshot_17.png){#fig:017 width=70%}

![Попытка прочитать файл /etc/shadow (неуспешно)](image/Screenshot_18.png){#fig:018 width=70%}

2. Исследование Sticky-бита (рис. [-@fig:019] - [-@fig:032]).

![Проверка, установлен ли атрибут Sticky на директории /tmp](image/Screenshot_19.png){#fig:019 width=70%}

![Создание файла file01.txt в директории /tmp](image/Screenshot_20.png){#fig:020 width=70%}

![Просмотр атрибутов и изменение прав](image/Screenshot_21.png){#fig:021 width=70%}

![Попытка прочитать файл](image/Screenshot_22.png){#fig:022 width=70%}

![Попытка дозаписать в файл /tmp/file01.txt слово test2 (отказ в доступе)](image/Screenshot_23.png){#fig:023 width=70%}

![Чтение файла](image/Screenshot_24.png){#fig:024 width=70%}

![Попытка записать в файл /tmp/file01.txt слово test3](image/Screenshot_25.png){#fig:025 width=70%}

![Чтение файла](image/Screenshot_26.png){#fig:026 width=70%}

![Попытка удалить файл /tmp/file01.txt](image/Screenshot_27.png){#fig:027 width=70%}

![Изменение прав](image/Screenshot_28.png){#fig:028 width=70%}

![Снятие режима суперпользователя](image/Screenshot_29.png){#fig:029 width=70%}

![Проверка атрибутов](image/Screenshot_30.png){#fig:030 width=70%}

![Попытка изменить файл (неуспешно), удалить файл (успешно)](image/Screenshot_31.png){#fig:031 width=70%}

![Возвращение атрибута](image/Screenshot_32.png){#fig:032 width=70%}

# Выводы

Я изучила механизмов изменения идентификаторов, применения SetUID- и Sticky-битов, получила практические навыки работы в консоли с дополнительными атрибутами, рассмотрела работу механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.
