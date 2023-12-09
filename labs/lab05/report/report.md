---
## Front matter
title: "Шаблон отчёта по лабораторной работе №5"
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

Приобретение практических навыков работы в Midnight Commander. Освоение инструкций языка ассемблера mov и int.

# Выполнение лабораторной работы

Открываю Midnight Commander, используя команду mc в Терминале, и перехожу в каталог "~/work/arch-pc" (рис. @fig:001).

![Открытие](image/001.jpg){#fig:001 width=70%}

Пользуясь клавишей F7, создаю папку lab05 и перехожу в созданный каталог. (рис. @fig:002).

![Создание папки lab05](image/002.jpg){#fig:002 width=70%}

В созданном каталоге создаю файл lab5-1.asm. Открываю его во встроенном редакторе, используя клавишу F4 (рис. @fig:003).

![Создание файла lab5-1.asm](image/003.jpg){#fig:003 width=70%}

Ввожу текст программы в файле lab5-1.asm. (рис. @fig:004).

![Текст программы в файле lab5-1.asm](image/00040444.jpg){#fig:004 width=70%}

Оттранслирую текст программы lab5-1.asm в объектный файл, после выполняю его компоновку и запускаю получившееся. Ввожу с клавиатуры свои ФИО. (рис. @fig:005).

![Компоновка файла lab5-1.asm.](image/005.jpg){#fig:005 width=70%}

Скачиваю файл in_out.asm с ТУИС и копирую его в папку lab05, используя клавишу F5. (рис. @fig:006).

![Скачивание файла in_out.asm](image/006.jpg){#fig:006 width=70%}

При помощи клавиши F5, создаю копию файла lab5-1.asm с названием "lab5-2.asm". (рис. @fig:007).

![Копия файла lab5-1.asm.](image/007.jpg){#fig:007 width=70%}

Исправляю текст программы файла lab5-2.asm с использованием подпрограмм файла in_out.asm. (рис. @fig:008).

![Текст программы файла lab5-2.asm.](image/008.jpg){#fig:008 width=70%}

Создаю исполняемый файл и проверяю его работу. (рис. @fig:009).

![Компоновка файла lab5-1.asm.](image/009.jpg){#fig:009 width=70%}

В файле lab5-2.asm заменяю подпрограмму sprintLF на sprint и проверяю результат работы нового исполняемого файла. Замечаю, что при вводе текста с клавиатуры строка перевода строки отсутствует. 

#Задания для самостоятельной работы

Создаю копию файла lab5-1.asm с названием "lab5-3.asm" и заменяю в нём программу по заданию. (рис. @fig:0010).

![Текст программы файла lab5-3.asm](image/0010.jpg){#fig:0010 width=70%} 

Проверяю результат работы. (рис. @fig:0011).

![Проверка результата](image/0011.jpg){#fig:0011 width=70%} 

Создаю копию файла lab5-2.asm с названием  "lab5-4.asm" и заменяю в нём программу по заданию. (рис. @fig:0013).

![Текст программы файла lab5-4.asm](image/0013.jpg){#fig:0013 width=70%} 

Проверяю результат работы. (рис. @fig:0012).

![Проверка результата](image/0012.jpg){#fig:0012 width=70%} 

# Вывод

Я приобрёл практические навыки работы в Midnight Commander и освоил инструкции языка ассемблера mov и int.


