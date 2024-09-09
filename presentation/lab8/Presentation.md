---
## Front matter
title: "Презентация по лабораторной работе №8"
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

- Освоить на практике применение режима однократного гаммирования на примере кодирования различных исходных текстов одним ключом


# Выполнение работы

1. Проанализировали паттерны работы самого шифрования/дешифрования.

2. В программе мы занесли ASCII таблицу в вектор.

3. Сделали генератор случайного ключа.

4. Написали функции шифрования/дешифрования.

5. Прописали главную функцию со всей логикой.

6. Получили в консоль информацию.

# Листинг программы 

## ASCII to Vector

![ASCII to Vector](../Report/img/1.png)

## Random key generator

![Random Key Generator](../Report/img/2.png)

## Encryption/Decryption methods

![Encryption/Decryption methods](../Report/img/3.png)

## Main

![Main function](../Report/img/4.png)

## Output

![Console output](../Report/img/5.png)

# Выводы

Во время выполнения работы, мы получили навыки работы с режимом однократного гаммирования и поняли, что в режиме однократного гамирования получить второй текст можно легко узнать чужой исходный текст, зная, например, свой зашифрованный текст и исходный текст и чужой зашифрованный текст. 

# Спасибо за вниманиие