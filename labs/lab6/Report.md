---
## Front matter
title: "Отчёт по лабораторной работе №6"
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

- Развить навыки администрирования ОС Linux. Получить первое практическое знакомство с технологией SELinux.

- Проверить работу SELinx на практике совместно с веб-сервером Apache.

# Выполнение работы

1. Проверили работу SELinux, что она работает.

2. Прописали в /etc/httpd/conf/httpd.conf ServerName:test.ru.

3. Создали test.html в /var/www/html и прописали простенькую форму и проверили с переходом на 127.0.0.1:80/test.html

4. Изменили контекст html файла на samba_share_t и узнали, что нет доступа к странице.

5. Изменили порт на 81 и узнали, что над прописывать :81 к ip или делать привязку к http_port_t.

6. Вернули порт на 80 и удалили привязку http_port_t к 81.

# Заключение

Во время выполнения работы, мы получили практические навыки работы с Apache Http Server.