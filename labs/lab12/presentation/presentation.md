---
## Front matter
lang: ru-RU
title: Лабораторная работа 12
subtitle: Настройка NAT
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

Приобретение практических навыков по настройке доступа локальной сети к внешней сети посредством NAT.

## Задание

1. Сделать первоначальную настройку маршрутизатора provider-gw-1 и коммутатора provider-sw-1 провайдера: задать имя, настроить доступ по паролю и т.п.
2. Настроить интерфейсы маршрутизатора provider-gw-1 и коммутатора provider-sw-1 провайдера: 
3. Настроить интерфейсы маршрутизатора сети «Донская» для доступа к сети провайдера.
4. Настроить на маршрутизаторе сети «Донская» NAT с правилами, указанными в разделе 12.2.
5. Настроить доступ из внешней сети в локальную сеть организации, как указано в разделе 12.2.
6. Проверить работоспособность заданных настроек.
  
  ## Заданиеы

# Выполнение лабораторной работы

## Выполнение лабораторной работы

![Первоначальная настройка маршрутизатора provider-yalantsova-gw-1](image/1.png){#fig:001 width=50%}

## Выполнение лабораторной работы

![Первоначальная настройка коммутатора provider-yalantsova-sw-1](image/2.png){#fig:002 width=60%}

## Выполнение лабораторной работы

![Настройка интерфейсов маршрутизатора provider-yalantsova-gw-1](image/3.png){#fig:003 width=40%}

## Выполнение лабораторной работы

![Настройка интерфейсов коммутатора provider-yalantsova-sw-1](image/4.png){#fig:004 width=40%}

## Выполнение лабораторной работы

![Настройка интерфейсов маршрутизатора msk-donskaya-yalantsova-gw-1](image/5.png){#fig:005 width=40%}

## Выполнение лабораторной работы

![Проверка связи между маршрутизаторами](image/6.png){#fig:006 width=60%}

## Выполнение лабораторной работы

![Настройка пула адресов для NAT](image/7.png){#fig:007 width=60%}

## Выполнение лабораторной работы

![Оборудование в здании сети модельного Интернета](image/8.png){#fig:008 width=60%}

## Выполнение лабораторной работы

![Настройка PAT](image/9.png){#fig:009 width=50%}

## Выполнение лабораторной работы

![Схема сети Интернет с ноутбуком](image/10.png){#fig:010 width=60%}

## Выполнение лабораторной работы

![Настройка доступа из Интернета](image/11.png){#fig:011 width=70%}

## Выполнение лабораторной работы

![Доступ dk-donskaya-1 к www.yandex.ru](image/12.png){#fig:012 width=50%}

## Выполнение лабораторной работы

![Доступ dk-donskaya-1 к esystem.pfur.ru](image/13.png){#fig:013 width=50%}

## Выполнение лабораторной работы

![Доступ dep-donskaya-1 к www.yandex.ru](image/14.png){#fig:014 width=50%}

## Выполнение лабораторной работы

![Доступ dep-donskaya-1 к esystem.pfur.ru](image/15.png){#fig:015 width=50%}

## Выполнение лабораторной работы

![Проверка доступа из Интернета по ftp](image/16.png){#fig:016 width=35%}

## Выполнение лабораторной работы

![Проверка доступа из Интернета к web-серверу](image/17.png){#fig:017 width=50%}

## Выводы

В результате выполнения лабораторной были приобретены практические навыки по настройке доступа локальной сети к внешней сети посредством NAT.
