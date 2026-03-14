---
title: 'Лабораторная работа №5'

subtitle: 'дисциплина: Операционные системы'

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

Получение практических навыков работы с менеджером паролей pass, а также освоение инструмента управления конфигурационными файлами chezmoi.

# Задание

- Установить и настроить менеджер паролей pass
- Настроить синхронизацию хранилища паролей с git
- Установить дополнительное программное обеспечение и шрифты
- Установить и настроить chezmoi
- Создать репозиторий dotfiles и подключить его к системе

# Теоретическое введение

Менеджер паролей pass — программа, сделанная в рамках идеологии Unix. Данные хранятся в файловой системе в виде каталогов и файлов, которые шифруются с помощью GPG-ключа. Поддерживается синхронизация хранилища паролей через git.

chezmoi — инструмент для управления конфигурационными файлами домашнего каталога пользователя. Состояние файлов конфигурации сохраняется в каталоге ~/.local/share/chezmoi, который является клоном репозитория dotfiles. Поддерживает шаблоны и работу на нескольких машинах одновременно.

# Выполнение лабораторной работы

Устанавливаем менеджер паролей pass и pass-otp с помощью пакетного менеджера dnf. (рис. [-@fig:001])

![Установка pass и pass-otp](image/1.png){#fig:001 width=70%}

Инициализируем git-репозиторий для хранилища паролей и добавляем удалённый репозиторий. (рис. [-@fig:002])

![Добавление удалённого репозитория pass](image/2.png){#fig:002 width=70%}

Указываем адрес удалённого репозитория на GitHub для синхронизации хранилища паролей. (рис. [-@fig:003])

![Указание адреса репозитория](image/3.png){#fig:003 width=70%}

Устанавливаем дополнительное программное обеспечение, необходимое для настройки рабочей среды, а также шрифты iosevka. 

Устанавливаем chezmoi (рис. [-@fig:004])

![Установка chezmoi](image/4.png){#fig:004 width=70%}

Создаём репозиторий dotfiles на основе шаблона и инициализируем chezmoi, подключив его к репозиторию на GitHub. (рис. [-@fig:005])

![Создание репозитория и инициализация chezmoi](image/5.png){#fig:005 width=70%}

# Выводы

В результате выполнения лабораторной работы были получены практические навыки работы с менеджером паролей pass и инструментом управления конфигурационными файлами chezmoi. Настроена синхронизация хранилища паролей с git, установлено дополнительное программное обеспечение и шрифты, создан репозиторий dotfiles и подключён к системе.

# Список литературы{.unnumbered}

::: {#refs}
:::
