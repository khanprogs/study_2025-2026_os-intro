---
title: 'Лабораторная работа №1'

subtitle: 'дисциплина: Архитектура компьютера'

author: 'Хан Георгий Игоревич'


lang: ru-RU
toc-title: 'Содержание'


bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl


toc: true 
toc-depth: 2
lof: true 
lot: true 
fontsize: 13pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt

polyglossia-lang:
  name: russian
  options:
    - spelling=modern
    - babelshorthands=true
polyglossia-otherlangs:
  name: english

babel-lang: russian
babel-otherlangs: english

mainfont: Times New Roman
sansfont: Times New Roman
monofont: Times New Roman
mathfont: Times New Roman
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:

biblatex: true
biblio-style: 'gost-numeric'
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric

figureTitle: 'Рис.'
tableTitle: 'Таблица'
listingTitle: 'Листинг'
lofTitle: 'Список иллюстраций'
lotTitle: 'Список таблиц'
lolTitle: 'Листинги'

indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} 
  - \floatplacement{figure}{H} 
---

# Цель работы

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

- Установка Linux на VirtualBox
- Установка необходимого ПО
- Первоначальная настройка системы

# Теоретическое введение

Oracle VirtualBox — это программное обеспечение с открытым исходным кодом для виртуализации, позволяющее создавать и запускать виртуальные машины на компьютере с любой популярной операционной системой. Простыми словами, это программа, которая создаёт "компьютер внутри компьютера", где можно установить другую операционную систему, не затрагивая основную.

Виртуализация через VirtualBox создаёт изолированную среду, которая эмулирует аппаратное обеспечение компьютера. Это позволяет запускать полноценную операционную систему внутри вашей основной системы.

# Выполнение лабораторной работы

Установка Linux Fedora sway на VirtualBox. (рис. 1)

![Система Fedora sway](image/1.png){#fig:001 width=70%}

После запуска виртуальной машины устанавливаю средства разработки. (рис. 2)

![Установка средств разработки](image/2.png){#fig:003 width=70%}

Обновление пакетов. (рис. 3)

![Выполнение команды sudo dnf -y update](image/3.png){#fig:004 width=70%}

Внутри виртуальной машины добавляю своего пользователя в группу vboxsf, В хостовой системе подключаю разделяемую папку. (рис. 4)


![Выполнение установки](image/4.png){#fig:006 width=70%}

# Домашнее задание

С помощью команд получаю информацию о системе. (рис. 5)

![uname -r и lscpu (информация о ядре)](image/5.png){#fig:007 width=70%}

# Выводы

В ходе выполнения лабораторной работы я приобрел навыки установки виртуальной машины на VirtualBox, установил ряд пакетов и настроил OC для дальнейшей работы.

# Список литературы
- игнат
