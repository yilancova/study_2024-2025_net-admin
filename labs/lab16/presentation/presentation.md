---
## Front matter
lang: ru-RU
title: Лабораторная работа 16
subtitle: Настройка VPN
author:
  - Ланцова Я. И.
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - \usepackage{fontspec}
 - \usepackage{polyglossia}
 - \setmainlanguage{russian}
 - \setotherlanguage{english}
 - \newfontfamily\cyrillicfont{Arial}
 - \newfontfamily\cyrillicfontsf{Arial}
 - \newfontfamily\cyrillicfonttt{Arial}
 - \setmainfont{Arial}
 - \setsansfont{Arial}
 
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Ланцова Яна Игоревна
  * студентка
  * Российский университет дружбы народов

:::
::::::::::::::

## Цель работы

Получение навыков настройки VPN-туннеля через незащищённое Интернет-соединение.

## Задание

Настроить VPN-туннель между сетью Университета г. Пиза (Италия) и сетью «Донская» в г. Москваs

# Выполнение лабораторной работы

# Размещение оборудования

## Выполнение лабораторной работы

![Схема сети](image/1.png){#fig:001 width=50%}

## Выполнение лабораторной работы

![Города сети](image/2.png){#fig:002 width=50%}

## Выполнение лабораторной работы

![Физическая область города Пиза](image/3.png){#fig:003 width=50%}

# Первоначальная настройка оборудования

## Выполнение лабораторной работы

![Настройка маршрутизатора pisa-unipi-yalantsova-gw-1](image/4.png){#fig:004 width=50%}

## Выполнение лабораторной работы

![Настройка коммутатора pisa-unipi-yalantsova-sw-1](image/5.png){#fig:005 width=50%}

## Выполнение лабораторной работы

![Настройка интерфейсов маршрутизатора pisa-unipi-yalantsova-gw-1](image/6.png){#fig:006 width=50%}

## Выполнение лабораторной работы

![Настройка интерфейсов маршрутизатора pisa-unipi-yalantsova-sw-1](image/7.png){#fig:007 width=50%}

# Настройка VPN на основе GRE

## Выполнение лабораторной работы

![Проверка связи между устройствами в городе Пиза](image/8.png){#fig:008 width=50%}

## Выполнение лабораторной работы

![Настройка VPN на маршрутизаторе msk-donskaya-yalantsova-gw-1](image/9.png){#fig:009 width=50%}

## Выполнение лабораторной работы

![Настройка VPN на маршрутизаторе pisa-unipi-yalantsova-gw-1](image/10.png){#fig:010 width=50%}

## Выполнение лабораторной работы

![Проверка доступности узлов сети Университета г. Пиза из сети Донская](image/11.png){#fig:011 width=50%}

# Выводы

В результате выполнения лабораторной были приобретены практические навыки по настройке VPN-туннеля через незащищённое Интернет-соединение.
