---
# Front matter
lang: ru-RU
title: "Отчёта по лабораторной работе №2"
subtitle: "Управление версиями"
author: "Башкирова Я.Д"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы
изучить идеологию и применение средств контроля версий.

# Задачи
1. Настройка git
2. Подключение репозитория к github
3. Первичная конфигурация
4. Конфигурация git-flow

# Ход работы
## Настройка git:
Создаем учетную запись на github
![](image/01.png){ #fig:001 width=70% }

Настраиваем систему контроля версий git: для этого генерирум ключ с помощью команды ssh-keygen -C «Имя Фамилия <work@mail>», загружаем сгенерённый ключ на github, далее, скопировав из локальной консоли ключ в буфер обмена с помощью команды cat ~/.ssh/id_rsa.pub | xclip -sel clip, вставляем ключ в появившееся на сайте поле.
![](image/02.png){ #fig:001 width=70% }
![](image/03.png){ #fig:001 width=70% }

## Подключение репозитория к github:
Создаём репозиторий на github:
![](image/04.png){ #fig:001 width=70% }

Переходим в рабочий каталог laboratory:
![](image/05.png){ #fig:001 width=70% }

Инициализируем системы git:
![](image/07.png){ #fig:001 width=70% }

Создаём заготовку для файла README.md:
![](image/08.png){ #fig:001 width=70% }

Делаем первый коммит и выкладываем на github:
![](image/09.png){ #fig:001 width=70% }
![](image/10.png){ #fig:001 width=70% }

## Первичная конфигурация:

Добавим файл лицензии:
![](image/11.png){ #fig:001 width=70% }

Добавим шаблон игнорируемых файлов и просмотрим список имеющихся шаблонов:
![](image/12.png){ #fig:001 width=70% }

Затем скачаем шаблон:
![](image/13.png){ #fig:001 width=70% }

Добавим новые файлы:
![](image/14.png){ #fig:001 width=70% }

Выполним коммит:
![](image/15.png){ #fig:001 width=70% }

Отправим на github:
![](image/16.png){ #fig:001 width=70% }

## Конфигурация git-flow:
Инициализируем git-flow:
![](image/17.png){ #fig:001 width=70% }

Проверим, что мы на ветке develop:
![](image/18.png){ #fig:001 width=70% }

Создадим релиз с версией 1.0.0:
![](image/19.png){ #fig:001 width=70% }

Запишем версию:
![](image/20.png){ #fig:001 width=70% }

Добавим в индекс:
![](image/21.png){ #fig:001 width=70% }

Зальём релизную ветку в основную ветку:
![](image/22.png){ #fig:001 width=70% }

Отправим данные на github:
![](image/23.png){ #fig:001 width=70% }

Создадим релиз на github:
![](image/24.png){ #fig:001 width=70% }

# Выводы
я изучила идеологию и применение средств контроля версий, научилась генерировать ключи и подключать репозиторий.

