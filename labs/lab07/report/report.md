---
## Front matter
title: "Лабораторная работа 7"
subtitle: "Учёт физических параметров сети"
author: "Ланцова Яна Игоревна"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Получить навыки работы с физической рабочей областью Packet Tracer, а также учесть физические параметры сети.

# Задание

Требуется заменить соединение между коммутаторами двух территорий msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1 на соединение, учитывающее физические параметры сети, а именно — расстояние между двумя территориями.

# Выполнение лабораторной работы

Откроем проект прошлой лабораторной работы(рис. [-@fig:001]).

![Схема сети без учёта физических параметров сети в логической рабочей области Packet Tracer](image/1.png){#fig:001 width=70%}

Перейдем в физическую рабочую область Packet Tracer. Присвоим название городу -- Moscow(рис. [-@fig:002]).

![Физическая рабочая область Packet Tracer](image/2.png){#fig:002 width=70%}

Щёлкнув на изображении города, увидим изображение здания. Присвоим ему название Donskaya. Добавим здание для территории Pavlovskaya(рис. [-@fig:003]).

![Изображение здания в физической рабочей области Packet Tracer (сеть территории «Донская»)](image/3.png){#fig:003 width=70%}

Щёлкнув на изображении здания Donskaya, переместим изображение, обозначающее серверное помещение, в него(рис. [-@fig:004]).

![Пример размещения в физической рабочей области Packet Tracer серверной с подключением оконечных устройств (сеть территории «Донская»)](image/4.png){#fig:004 width=70%}

Щёлкнув на изображении серверной, посмотрим отображение серверных стоек(рис. [-@fig:005]).

![Отображение серверных стоек в Packet Tracer](image/5.png){#fig:005 width=70%}

Переместим коммутатор msk-pavlovskaya-yalantsova-sw-1 и два оконечных устройства dk-pavlovskaya-yalantsova-1 и other-pavlovskaya-yalantsova-1 на территорию Pavlovskaya, используя меню Move физической рабочей области Packet Tracer (рис. [-@fig:006]).

![Перемещение устройств на территорию Pavlovskaya](image/6.png){#fig:006 width=70%}

Вернувшись в логическую рабочую область Packet Tracer, пропингуем с коммутатора msk-donskaya-yalantsova-sw-1 коммутатор msk-pavlovskaya-yalantsova-sw-1. Убедимся, что соединение работоспособно(рис. [-@fig:007]).

![Проверка работоспособности соединения между msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1](image/7.png){#fig:007 width=70%}

В меню Options, Preferences во вкладке Interface активируем разрешение на учёт физических характеристик среды передачи (Enable Cable Length Effects)(рис. [-@fig:008]).

![Активация разрешения на учёт физических характеристик среды передачи](image/8.png){#fig:008 width=70%}

В физической рабочей области Packet Tracer разместим две территории на расстоянии  около 1000 м друг от друга(рис. [-@fig:009]).

![Размешение территорий на расстоянии около 1000 м друг от друга](image/9.png){#fig:009 width=90%}

Вернувшись в логическую рабочую область Packet Tracer, пропингуем с коммутатора msk-donskaya-yalantsova-sw-1 коммутатор msk-pavlovskaya-yalantsova-sw-1. Убедимся, что соединение не работает(рис. [-@fig:010]).

![Проверка неработоспособности соединения между msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1](image/10.png){#fig:010 width=90%}

Удалим соединение между msk-donskaya-sw-1 и msk-pavlovskaya-sw-1. Добавим в логическую рабочую область два повторителя (Repeater-PT). Присвоим им соответствующие названия msk-donskaya-yalantsova-mc-1 и msk-pavlovskaya-yalantsova-mc-1. Заменим имеющиеся модули на PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE для подключения оптоволокна и витой пары по технологии Fast Ethernet(рис. [-@fig:011]).

![Замена модулей на репиторах для подключения оптоволокна и витой пары по технологии Fast Ethernet](image/11.png){#fig:011 width=90%}

Переместим msk-pavlovskaya-mc-1 на территорию Pavlovskaya (в физичекой рабочей области Packet Tracer).

Подключим коммутатор msk-donskaya-yalantsova-sw-1 к msk-donskaya-yalantsova-mc-1 по витой паре, msk-donskaya-yalantsova-mc-1 и msk-pavlovskaya-yalantsova-mc-1 -- по оптоволокну, msk-pavlovskaya-yalantsova-sw-1 к msk-pavlovskaya-yalantsova-mc-1 -- по витой паре(рис. [-@fig:012]).

![Схема сети c учётом физических параметров сети в логической рабочей области Packet Tracer](image/12.png){#fig:012 width=90%}

Перенесем репитор с Донской на Павловскую(рис. [-@fig:013]).

![Перенос репитора](image/13.png){#fig:013 width=90%}

Убедимся в работоспособности соединения междуmsk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1(рис. [-@fig:014]).

![Проверка работоспособности соединения между msk-donskaya-yalantsova-sw-1 и msk-pavlovskaya-yalantsova-sw-1](image/14.png){#fig:014 width=90%}


# Выводы

В результате выполнения лабораторной работы получили навыки работы с физической рабочей областью Packet Tracer, а также учесть физические параметры сети.

# Контрольные вопросы

1. Перечислите возможные среды передачи данных. На какие характеристики
среды передачи данных следует обращать внимание при планировании
сети?
2. Перечислите категории витой пары. Чем они отличаются? Какая категория
в каких условиях может применяться?
3. В чем отличие одномодового и многомодового оптоволокна? Какой тип
кабеля в каких условиях может применяться?
4. Какие разъёмы встречаются на патчах оптоволокна? Чем они отличаются?

1. Среды передачи данных: проводная (витая пара, коаксиальный кабель, оптоволокно), беспроводная (Wi-Fi, Bluetooth, сотовая связь). При планировании сети следует обращать внимание на пропускную способность каналов передачи данных, задержку (латентность), надежность соединения, уровень шума и помех, а также возможность интерференции сигналов.

2. Категории витой пары: Cat5, Cat6, Cat6a, Cat7. Они отличаются пропускной способностью и дальностью передачи. Cat5 подходит для домашних сетей, Cat6 для офисов, Cat6a и Cat7 для высокоскоростных сетей.

3. Одномодовое оптоволокно передает свет в одном направлении, многомодовое - в нескольких. Одномодовое используется на большие расстояния, многомодовое - на короткие.

4. Разъемы на патчах оптоволокна: LC, SC, ST. Они различаются по типу соединения. LC - для высокоскоростных сетей, SC и ST - для обычных сетей.
