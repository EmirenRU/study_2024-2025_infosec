---
## Front matter
title: "Отчёт по лабораторной работе №8"
subtitle: "НКНбд-01-21"
author: "Юсупов Эмиль Артурович"

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
linestretch: 1.25
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
mainfont: Open Sans
romanfont: Open Sans
sansfont: Open Sans
monofont: Open Sans
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

# Введение

## Цель работы

- Освоить на практике применение режима однократного гаммирования на примере кодирования различных исходных текстов одним ключом

# Выполнение работы

1. Проанализировали паттерны работы самого шифрования/дешифрования.

2. В программе мы занесли ASCII таблицу в вектор.

![ASCII to Vector](../Report/img/1.png)

3. Сделали генератор случайного ключа.

![Random Key Generator](../Report/img/2.png)

4. Написали функции шифрования/дешифрования.

![Encryption/Decryption methods](../Report/img/3.png)

5. Прописали главную функцию со всей логикой.

![Main function](../Report/img/4.png)

6. Получили в консоль информацию.

![Console output](../Report/img/5.png)

# Заключение

Во время выполнения работы, мы получили навыки работы с режимом однократного гаммирования и поняли, что в режиме однократного гамирования получить второй текст можно легко узнать чужой исходный текст, зная, например, свой зашифрованный текст и исходный текст и чужой зашифрованный текст. 