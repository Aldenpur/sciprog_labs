---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: "Дисциплина: Научное программирование"
author: "Дэнэилэ Александр Дмитриевич, НПМмд-02-23"

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

Ознакомиться с основами работы с системами линейных уравнений в GNU Octave.

# Задание

1. Ознакомиться с реализацией метода Гаусса.
1. Изучить метод левого деления.
1. Ознакомиться с LU-разложением и LUP-разложением.


# Выполнение лабораторной работы

1. Ознакомился с методами обращения как к отдельному элементу, так и к целой строке/столбцу матрицы. Реализовал метод Гаусса. Вывел получившуюся треугольную матрицу в коротком и длинном формате (рис. @fig:001).

![Метод Гаусса](image/1.png){#fig:001 width=60%}

2. Реализуем метод левого деления, разбив расширенную матрицу *B* на квадратную матрицу *A* и вектор-столбец *b* . (рис. @fig:002).

![Левое деление](image/2.png){#fig:002 width=60%}


3. Реализуем LU-разложение матрицы *С* (рис. @fig:003).

![LU-разложение матрицы ](image/3.png){#fig:003 width=60%}

4. Реализуем LUP-разложение матрицы *С* (рис. @fig:004).

![LUP-разложение матрицы ](image/4.png){#fig:004 width=60%}

# Выводы

Научился работе с системами линейных алгебраических уравнений в Octave.

# Список литературы{.unnumbered}

::: {#refs}
:::
