---
## Front matter
lang: ru-RU
title: Лабораторная работа 9
subtitle: Использование протокола STP. Агрегирование каналов
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

Изучение возможностей протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними.

## Задание

1. Сформируйте резервное соединение между коммутаторами msk-donskaya-sw-1 и msk-donskaya-sw-3.
2. Настройте балансировку нагрузки между резервными соединениями.
3. Настройте режим Portfast на тех интерфейсах коммутаторов, к которым подключены серверы.
4. Изучите отказоустойчивость резервного соединения.
5. Сформируйте и настройте агрегированное соединение интерфейсов Fa0/20 -- Fa0/23 между коммутаторами msk-donskaya-sw-1 и msk-donskaya-sw-4.

# Выполнение лабораторной работы

## Выполнение лабораторной работы

![Схема сети в логической рабочей области Packet Tracer](image/1.png){#fig:001 width=60%}

## Выполнение лабораторной работы

![настройка порта на коммутаторе msk-donskaya-yalantsova-sw-3](image/2.png){#fig:002 width=70%}

## Выполнение лабораторной работы

![настройка порта на коммутаторе msk-donskaya-yalantsova-sw-1](image/3.png){#fig:003 width=70%}

## Выполнение лабораторной работы

![настройка порта на коммутаторе msk-donskaya-yalantsova-sw-4](image/4.png){#fig:004 width=70%}

## Выполнение лабораторной работы

![Логическая схема локальной сети с резервным соединением](image/5.png){#fig:005 width=50%}

## Выполнение лабораторной работы

![Проверка доступности устройств с помощью команды `ping`](image/6.png){#fig:006 width=70%}

## Выполнение лабораторной работы

![Проверка доступности устройств в режиме симуляции](image/7.png){#fig:007 width=60%}

## Выполнение лабораторной работы

![Просмотр информации о STP для vlan 3 на msk-pavlovskaya-yalantsova-sw-1](image/8.png){#fig:008 width=60%}

## Выполнение лабораторной работы

![Проверка пути от хоста dk-donskaya-1 до mail](image/9.png){#fig:009 width=60%}

## Выполнение лабораторной работы

![Проверка пути от хоста dk-donskaya-1 до web](image/10.png){#fig:010 width=60%}

## Выполнение лабораторной работы

![Настройка режима Portfast на msk-donskaya-yalantsova-sw-2](image/11.png){#fig:011 width=60%}

## Выполнение лабораторной работы

![Настройка режима Portfast на msk-donskaya-yalantsova-sw-3](image/12.png){#fig:012 width=60%}

## Выполнение лабораторной работы

![Изучение отказоустойчивости протокола STP и время восстановления соединения](image/13.png){#fig:013 width=60%}

## Выполнение лабораторной работы

```
msk-donskaya-yalantsova-sw-1( config )#spanning-tree mode rapid-pvst
msk-donskaya-yalantsova-sw-2( config )#spanning-tree mode rapid-pvst
msk-donskaya-yalantsova-sw-3( config )#spanning-tree mode rapid-pvst
msk-donskaya-yalantsova-sw-4( config )#spanning-tree mode rapid-pvst
msk-pavlovskaya-yalantsova-sw-1( config )#spanning-tree mode rapid-pvst
```

## Выполнение лабораторной работы

![Изучение отказоустойчивость протокола Rapid PVST+ и время восстановления соединения](image/14.png){#fig:014 width=70%}

## Выполнение лабораторной работы

![Логическая схема локальной сети с агрегированным соединением](image/15.png){#fig:015 width=50%}

## Выполнение лабораторной работы

![Настройка агрегирования каналов на msk-donskaya-yalantsova-sw-1](image/16.png){#fig:016 width=50%}

## Выполнение лабораторной работы

![Настройка агрегирования каналов на msk-donskaya-yalantsova-sw-1](image/17.png){#fig:017 width=70%}

## Выводы

В результате выполнения лабораторной работы изучили возможности протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними.
