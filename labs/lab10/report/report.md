---
## Front matter
title: "Лабораторная работа №10"
subtitle: "Простейший вариант"
author: "Бадалов Заури Эльвин оглы"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Приобрести навыки работы с файлами на языке NASM и научиться управлять правами доступа к файлу.

# Выполнение лабораторной работы

Создаю файл lab10-1.asm в рабочей директории lab10. (рис. @fig:001).

![Создание файла lab10-1.asm](image/221.jpg){#fig:001 width=70%}

Записываю в файл lab10-1.asm текст программы. (рис. @fig:002).

![Текст программы в lab10-1.asm](image/222.jpg){#fig:002 width=70%}

Проверяю работу программы. (рис. @fig:003).

![Запуск программы](image/223.jpg){#fig:003 width=70%}

Запрещаю исполнение для файла lab10-1.asm. (рис. @fig:004).

![Запрет исполнения файла lab10-1.asm](image/224.jpg){#fig:004 width=70%}

Как следствие, не получается исполнить этот файл.

При разрешении исполнения файла с расширением .asm и его исполнении, выводится большое количество ошибок. (рис. @fig:005).

![Разрешение исполнения файла lab10-1.asm](image/225.jpg){#fig:005 width=70%}

#Задания для самостоятельной работы

Пишу программу по заданию. (рис. @fig:006) и (рис. @fig:007).

![Текст программы в zadan10.asm (1)](image/226.jpg){#fig:006 width=70%}

![Текст программы в zadan10.asm (2)](image/227.jpg){#fig:007 width=70%}

Проверяю работу программы. (рис. @fig:008).

![Запуск программы](image/228.jpg){#fig:008 idth=70%}

# Выводы

Были приобретены навыки по рабте с файлами NASM и правами доступа к файлам.


