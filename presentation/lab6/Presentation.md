---
## Front matter
title: "Презентация по лабораторной работе №6"
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

- Развить навыки администрирования ОС Linux. Получить первое практическое знакомство с технологией SELinux.

- Проверить работу SELinx на практике совместно с веб-сервером Apache.

# Выполнение работы

1. Проверили работу SELinux, что она работает.

2. Прописали в /etc/httpd/conf/httpd.conf ServerName:test.ru.

3. Создали test.html в /var/www/html и прописали простенькую форму и проверили с переходом на 127.0.0.1:80/test.html

4. Изменили контекст html файла на samba_share_t и узнали, что нет доступа к странице.

5. Изменили порт на 81 и узнали, что над прописывать :81 к ip или делать привязку к http_port_t.

6. Вернули порт на 80 и удалили привязку http_port_t к 81.

# Выводы

Во время выполнения работы, мы получили практические навыки работы с Apache Http Server.

# Спасибо за вниманиие