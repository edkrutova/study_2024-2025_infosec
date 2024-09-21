---
## Front matter
lang: ru-RU
title: Лабораторная работа №3
subtitle: Дискреционное разграничение прав в Linux. Два пользователя
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

Целью данной работы является приобретение практических навыков работы в консоли с атрибутами файлов для групп пользователей.

# Выполнение работы 1

![Создание учётной записи пользователя guest](image/Screenshot_1.png){#fig:001 width=40%}

![Пароль пользователя guest](image/Screenshot_2.png){#fig:002 width=40%}

![Создание учётной записи пользователя guest2](image/Screenshot_3.png){#fig:003 width=40%}

# Выполнение работы 2

![Добавление пользователя guest2 в группу guest](image/Screenshot_4.png){#fig:004 width=40%}

![Вход от guest и guest2](image/Screenshot_5.png){#fig:005 width=40%}

# Выполнение работы 3

![Определление директории guest](image/Screenshot_6.png){#fig:006 width=40%}

![Определене директории guest2](image/Screenshot_7.png){#fig:007 width=40%}

# Выполнение работы 4

![имя пользователя guest, его группа, а также группы, куда входит пользователь](image/Screenshot_8.png){#fig:008 width=50%}

![имя пользователя guest2, его группа, а также группы, куда входит пользователь](image/Screenshot_9.png){#fig:009 width=50%}

# Выполнение работы 5

![Просмотр файла /etc/passwd](image/Screenshot_10.png){#fig:010 width=70%}

# Выполнение работы 6

![Регистрация пользователя guest2 в группе guest](image/Screenshot_11.png){#fig:011 width=70%}

![Изменение прав директории /home/guest](image/Screenshot_12.png){#fig:012 width=70%}

![Снятие с директории /home/guest/dir1 всех атрибутов](image/Screenshot_13.png){#fig:013 width=70%}


# Заполнение таблицы

![Таблица](image/Screenshot_14.png){#fig:014 width=70%}

# Выводы

Я приобрела практические навыки работы в консоли с атрибутами файлов для групп пользователей.