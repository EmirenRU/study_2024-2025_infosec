---
## Front matter
title: "Презентация по индивидуальном проекте №2"
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

- Установить DAMN VULNERABLE WEB APPLICATION (DVWA) на kali linux и просмотреть, что в нем есть.


# Выполнение работы

1. Установили в дистрибутив DVWA через скрипт 

```bash
sudo bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/IamCarron/DVWA-Script/main/Install-DVWA.sh)"
```

2. Зашли в localhost/DVWA/setup.php и запустили настройку.

3. Вошли в admin:password в localhost/DVWA/login.php

4. Просмотрели, что находится в самом веб-приложении.

# Выводы

Во время выполнения работы, мы установили для дальнейшей работы DVWA и просмотрели, какие уязвимости бывают.

# Спасибо за вниманиие