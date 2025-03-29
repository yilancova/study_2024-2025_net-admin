---
## Front matter
lang: ru-RU
title: Лабораторная работа 7
subtitle: Учёт физических параметров сети
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

Получить навыки работы с физической рабочей областью Packet Tracer, а также учесть физические параметры сети.

## Задание

Требуется заменить соединение между коммутаторами двух территорий msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1 на соединение, учитывающее физические параметры сети, а именно — расстояние между двумя территориями.

# Выполнение лабораторной работы

## Выполнение лабораторной работы

![Схема сети без учёта физических параметров сети в логической рабочей области Packet Tracer](image/1.png){#fig:001 width=60%}

## Выполнение лабораторной работы

![Физическая рабочая область Packet Tracer](image/2.png){#fig:002 width=50%}

## Выполнение лабораторной работы

![Изображение здания в физической рабочей области Packet Tracer (сеть территории «Донская»)](image/3.png){#fig:003 width=70%}

## Выполнение лабораторной работы

![Пример размещения в физической рабочей области Packet Tracer серверной с подключением оконечных устройств (сеть территории «Донская»)](image/4.png){#fig:004 width=50%}

## Выполнение лабораторной работы

![Отображение серверных стоек в Packet Tracer](image/5.png){#fig:005 width=30%}

## Выполнение лабораторной работы

![Перемещение устройств на территорию Pavlovskaya](image/6.png){#fig:006 width=70%}

## Выполнение лабораторной работы

![Проверка работоспособности соединения между msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1](image/7.png){#fig:007 width=50%}

## Выполнение лабораторной работы

![Активация разрешения на учёт физических характеристик среды передачи](image/8.png){#fig:008 width=70%}

## Выполнение лабораторной работы

![Размешение территорий на расстоянии около 1000 м друг от друга](image/9.png){#fig:009 width=90%}

## Выполнение лабораторной работы

![Проверка неработоспособности соединения между msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1](image/10.png){#fig:010 width=90%}

## Выполнение лабораторной работы

![Замена модулей на репиторах для подключения оптоволокна и витой пары по технологии Fast Ethernet](image/11.png){#fig:011 width=90%}

## Выполнение лабораторной работы

![Схема сети c учётом физических параметров сети в логической рабочей области Packet Tracer](image/12.png){#fig:012 width=70%}

## Выполнение лабораторной работы

![Перенос репитора](image/13.png){#fig:013 width=90%}

## Выполнение лабораторной работы

![Проверка работоспособности соединения между msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1](image/14.png){#fig:014 width=90%}

## Выводы

В результате выполнения лабораторной работы получили навыки работы с физической рабочей областью Packet Tracer, а также учесть физические параметры сети.
