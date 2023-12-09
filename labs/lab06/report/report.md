---
## Front matter
title: "Шаблон отчёта по лабораторной работе №6"
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

Освоить арифметические инструкции языка ассемблера NASM.

# Выполнение лабораторной работы

Создаю каталог lab06, перехожу в него. (рис. @fig:001).

![Создание каталога lab06](image/0101.jpg){#fig:001 width=70%}

Cоздаю файл lab6-1.asm. (рис. @fig:002).

![Создание файла lab6-1.asm](image/0102.jpg){#fig:002 width=70%}

Пишу текст программы в файл lab6-1.asm. (рис. @fig:003).

![Текст программы в lab6-1.asm](image/0103.jpg){#fig:003 width=70%}

Создаю исполняемый файл и запускаю его. (рис. @fig:004).

![Запуск программы из lab6-1.asm](image/0104.jpg){#fig:004 width=70%}

Меняю определенные строки в тексте программы lab6-1.asm. (рис. @fig:005).

![Изменение программы в lab6-1.asm](image/0105.jpg){#fig:005 width=70%}

Создаю исполняемый файл уже с измененным текстом программы и запускаю его. (рис. @fig:006).

![Запуск измененной программы lab6-1.asm](image/0106.jpg){#fig:006 width=70%}

Создаю файл lab6-2.asm. (рис. @fig:007).

![Создание файла lab6-2.asm](image/0107.jpg){#fig:007 width=70%}

Вношу в файл lab6-2.asm текст программы. (рис. @fig:008).

![Текст программы в файле lab6-2.asm](image/0108.jpg){#fig:008 width=70%}

Создаю исполняемый файл и запускаю его. (рис. @fig:009).

![Запуск программы из lab6-2.asm](image/0109.jpg){#fig:009 width=70%}

Аналогично случаю с lab6-1.asm, заменю определенные символы на числа. (рис. @fig:0010).

![Изменение программы в lab6-2.asm](image/01010.jpg){#fig:0010 width=70%}

Запущу программу. (рис. @fig:0011).

![Запуск программы](image/01012.jpg){#fig:0011 width=70%}

Заменяю функцию iprintLF на iprint в файле lab6-2.asm. (рис. @fig:0012).

![Замена функции в тексте программы lab6-2.asm](image/01011.jpg){#fig:0012 width=70%}

Запускаю получившуюся программу. (рис. @fig:0013).

![Запуск программы](image/01013.jpg){#fig:0013 width=70%}

Создаю файл lab6-3.asm и ввожу туда текст программы. (рис. @fig:0014).

![Замена функции в тексте программы lab6-2.asm](image/01014.jpg){#fig:0014 width=70%}

Создаю исполняемый файл и запускаю его. (рис. @fig:0015).

![Запуск программы lab6-3.asm](image/01015.jpg){#fig:0015 width=70%}

Меняю текст программы в файле lab6-3.asm для вычисления выражения "f(x) = (4 * 6 + 2) / 5". (рис. @fig:0016).

![Вычисление выражения f(x) = (4 * 6 + 2) / 5](image/01016.jpg){#fig:0016 width=70%} 

Создаю файл variant.asm в том же каталоге. (рис. @fig:0017).

![Создание файла variant.asm](image/01017.jpg){#fig:0017 width=70%}

Ввожу текст программы в файл variant.asm. (рис. @fig:0018).

![Текст программы в variant.asm](image/01018.jpg){#fig:0018 width=70%}

Создаю исполняемый файл и запускаю программу. (рис. @fig:0019).

![Запуск программы variant.asm](image/01019.jpg){#fig:0019 width=70%}

Ответы на вопросы:

1) "mov eax, rem / call sprint"
2) Для ввода сообщения с клавиатуры.
3) Для преобразования ASCII-код в целое число.
4) "xor edx,edx / mov ebx,20 / div ebx / inc edx"
5) В регистр edx.
6) Для увеличения значения регистра edx на 1.
7) "mov eax,rem / call sprint / mov eax,edx / call iprintL. 

#Задание самостоятельной работы

Напишу программу вычисления выражения из 19 варианта. (рис. @fig:0020).

![Программа вычисления](image/01020.jpg){#fig:0020 width=70%}

Проверяю работу файла. (рис. @fig:0021).

![Запуск программы 19 варианта](image/01021.jpg){#fig:0021 width=70%}

# Вывод

Я освоил арифметические инструкции языка ассемблера NASM.

