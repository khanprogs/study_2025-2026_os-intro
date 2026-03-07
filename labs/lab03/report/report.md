---
title: 'Лабораторная работа №3'

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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

- Сделать отчет по предыдущей лабораторной работе в формате markdown
- В качестве отчета предоставить отчеты в 3 форматах: pdf, docx, md.

# Теоретическое введение

Чтобы создать заголовок,используйте знак (#)
Чтобы задатьдлятекста полужирное начертание,заключите его вдвойные звездочки
Чтобы задатьдлятекста курсивное начертание,заключите его в одинарные звездочки
Чтоб задать для текста полужирное и курсивное начертание, заключите его в тройные
звездочки
Неупорядоченный (маркированный) список можно отформатироватьс помощью звез
дочек илитире
Чтобы вложить один список в другой, добавьте отступ для элементов дочернего списка
Упорядоченный список можно отформатировать с помощью соответствующих цифр
Чтобы вложить один список в другой, добавьте отступ для элементов дочернего списка
Синтаксис Markdown для встроенно ссылки состоит из части
[link text] ,представляющей текст гиперссылки, и части
(file-name.md)–URL-адреса или имени файла,
на которыйдается ссылка
Markdown поддерживает как встраивание фрагментов кода в предложение,так и их
размещение между предложениями в виде отдельных огражденных блоков.Огражденные
блоки кода — это простой способ выделить синтаксис для фрагментов кода. Общий
формат огражденных блоков кода
Для обработки файлов в формате Markdown будем использовать Pandoc
https://pandoc.org/. Конкретно, нам понадобится программа pandoc,
pandoc-citeproc https://github.com/jgm/pandoc/releases, pandoc-crossref
https://github.com/lierdakil/pandoc-crossref/releases.

# Выполнение лабораторной работы

Открываю файл report.md через vs code. (рис. -1)

![Отчет](image/1.png){#fig:001 width=70%}

Указываю основную информацию о лабораторной работе. (рис. 2)

![Заполнение основной информации](image/2.png){#fig:002 width=70%}

# Выводы

В ходе выполнения лабораторной работы я научился оформлять отчеты с помощью языка разметки Markdown.

# Список литературы

- игнат