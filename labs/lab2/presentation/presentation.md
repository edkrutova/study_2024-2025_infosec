---
## Front matter
lang: ru-RU
title: Лабораторная работа №2
subtitle: Дискреционное разграничение прав в Linux. Основные атрибуты
author:
  - Крутова Е. Д.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 07 сентября 2024

babel-lang: russian
babel-otherlangs: english
mainfont: Arial
monofont: Courier New
fontsize: 10pt

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---


# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

* Крутова Екатерина Дмитриевна
* студентка группы НПИбд-01-21
* Российский университет дружбы народов
* [1032216536@pfur.ru](mailto:1032216536@pfur.ru)
* <https://edkrutova.github.io/ru/>

:::
::: {.column width="30%"}

![](./image/photo.jpg)

:::
::::::::::::::

# Цель работы

Целью данной работы является приобретение практических навыков работы в консоли с атрибутами файлов, закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux.

# Выполнение работы 1

![Создание учётной записи пользователя guest](image/Screenshot_1.png){#fig:001 width=40%}

![Пароль пользователя guest](image/Screenshot_2.png){#fig:002 width=40%}

![Вход от имени пользователя guest](image/Screenshot_3.png){#fig:003 width=40%}

# Выполнение работы 2

![Определение директории (домашняя)](image/Screenshot_4.png){#fig:004 width=40%}

![Имя пользователя](image/Screenshot_5.png){#fig:005 width=40%}

![имя пользователя, его группа, а также группы, куда входит пользователь](image/Screenshot_6.png){#fig:006 width=40%}

# Выполнение работы 3

![Просмотр файла /etc/passwd](image/Screenshot_7.png){#fig:007 width=40%}

uid пользователя 1001, gid пользователя 1001, совпадает.

![Существующие в системе директории](image/Screenshot_8.png){#fig:40 width=70%}

Права 700

# Выполнение работы 4

![Создание в домашней директории поддиректории dir1](image/Screenshot_10.png){#fig:009 width=70%}

![Снятие с директории dir1 всех атрибутов](image/Screenshot_11.png){#fig:010 width=70%}

![Попытка  создать в директории dir1 файл file1](image/Screenshot_12.png){#fig:011 width=70%}

# Заполнение таблицы

![таблица](image/Screenshot_14.png){#fig:012 width=70%}

# Выводы

Я приобрела практические навыки работы в консоли с атрибутами файлов, закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux.
