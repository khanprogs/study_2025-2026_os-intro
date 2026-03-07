---
title: 'Лабораторная работа №2'

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
Изучить идеологию и применение средств контроля версий и
освоить умения по работе с git.

# Задание

- базовая конфигурация для работы с git
- ключ SSH
- ключ PGP
- подписи git
- каталог для выполнения заданий

# Теоретическое введение

Системы контроля версий (Version Control System, VCS) применяются при работе нескольких человек над одним проектом. Обычно основное дерево проекта хранится в локальном или удалённом репозитории, к которому настроен доступ для участников проекта. При внесении изменений в содержание проекта система контроля версий позволяет их фиксировать, совмещать изменения, произведённые разными участниками проекта, производить откат к любой более ранней версии проекта, если это требуется.

В классических системах контроля версий используется централизованная модель, предполагающая наличие единого репозитория для хранения файлов. Выполнение большинства функций по управлению версиями осуществляется специальным сервером. Участник проекта (пользователь) перед началом работы посредством определённых команд получает нужную ему версию файлов. После внесения изменений, пользователь размещает новую версию в хранилище. При этом предыдущие версии не удаляются из центрального хранилища и к ним можно вернуться в любой момент. Сервер может сохранять не полную версию изменённых файлов, а производить так называемую дельта-компрессию — сохранять только изменения между последовательными версиями, что позволяет уменьшить объём хранимых данных.

# Выполнение лабораторной работы
Произвожу базовую настройку git. (рис. 1)

![Пример конфигурации git](image/1.png){#fig:001 width=70%}

Создаю ssh и gpg ключи. (рис. 2)

![Генерация ключей](image/2.png){#fig:002 width=70%}

Экспортирую gpg ключ для авторизации на github. (рис. 3)

![Экспорт ключа](image/3.png){#fig:004 width=70%}

Авторизуюсь на github для работы через терминал. (рис. 4)

![Авторизация на github](image/4.png){#fig:006 width=70%}

Создаю директорию курса по шаблону. (рис. 5)

![Создание директрории курса](image/5.png){#fig:007 width=70%}

Настраиваю рабочую директорию. (рис. 6)

![Настройка директории](image/6.png){#fig:008 width=70%}

# Выводы

В результате выполнения данной лабораторной работы я научился базовым навыкам работы с git: создание репозиториев, ssh и gpg ключе, настройка каталога курса и авторизация gh.

# Список литературы
- игнат
