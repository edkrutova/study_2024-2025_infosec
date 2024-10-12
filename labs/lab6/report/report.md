---
## Front matter
title: "Лабораторная работа №6"
subtitle: "Мандатное разграничение прав в Linux."
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

Целью данной работы является развитие навыков администрирования ОС Linux, получение первого практического знакомства с технологией SELinux.
Проверка работы SELinx на практике совместно с веб-сервером Apache.

# Выполнение лабораторной работы

1. Создание программы (рис. [-@fig:001] - [-@fig:023]).

![Проверка работы SELinux](image/Screenshot_1.png){#fig:001 width=70%}

![Проверка работы веб-сервера](image/Screenshot_2.png){#fig:002 width=70%}

![Просмотра контекста безопасности](image/Screenshot_3.png){#fig:003 width=70%}

![Просмотр текущего состояния переключателей SELinux](image/Screenshot_4.png){#fig:004 width=70%}

![Просмотр статистики по политике](image/Screenshot_5.png){#fig:005 width=70%}

![тип файлов и поддиректорий, находящихся в директории /var/www](image/Screenshot_6.png){#fig:006 width=70%}

![тип файлов, находящихся в директории /var/www/html](image/Screenshot_7.png){#fig:007 width=70%}

![/var/www/html/test.html](image/Screenshot_8.png){#fig:008 width=70%}

![Контекст файла](image/Screenshot_11.png){#fig:009 width=70%}

![Веб-сервер](image/Screenshot_10.png){#fig:010 width=70%}

![Проверка контекста файла](image/Screenshot_11.png){#fig:011 width=70%}

![Изменение контекста файла](image/Screenshot_12.png){#fig:012 width=70%}

![Ошибка доступа к веб-серверу](image/Screenshot_13.png){#fig:013 width=70%}

![Просмотр log-файлов веб-сервера Apache](image/Screenshot_14.png){#fig:014 width=70%}

![Изменение /etc/httpd/httpd.conf](image/Screenshot_15.png){#fig:015 width=70%}

![Перезапуск веб-сервера Apache](image/Screenshot_16.png){#fig:016 width=70%}

![Просмотр файла /var/log/http/error_log](image/Screenshot_17.png){#fig:017 width=70%}

![Возвращение контекста httpd_sys_cоntent__t к файлу /var/www/html/ test.html](image/Screenshot_18.png){#fig:018 width=70%}

![Перезапуск веб-сервера Apache](image/Screenshot_19.png){#fig:019 width=70%}

![Веб-сервер Apache](image/Screenshot_20.png){#fig:020 width=70%}

![Исправление конфигурационного файла apache](image/Screenshot_21.png){#fig:021 width=70%}

![Удаление привязки http_port_t к 81 порту](image/Screenshot_22.png){#fig:022 width=70%}

![Удаление файла /var/www/html/test.html](image/Screenshot_23.png){#fig:023 width=70%}

# Выводы

Я развила навыки администрирования ОС Linux, получила первое практическое знакомство с технологией SELinux.
Проверила работу SELinx на практике совместно с веб-сервером Apache.
