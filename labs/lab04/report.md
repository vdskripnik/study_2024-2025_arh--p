---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Архитектура компьютера"
author: "Скрипник Виктория Дмитриевна"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно про Unix см. в [@tanenbaum_book_modern-os_ru; @robbins_book_bash_en; @zarrelli_book_mastering-bash_en; @newham_book_learning-bash_en].

# Выполнение лабораторной работы

1. Создадим каталог для работы с программами на языке ассемблера NASM и перейдем в созданный каталог: (рис.1 [-@fig:001]).

![рис 1](image/1.png){#fig:001 width=70%}

2. Создадим текстовый файл с именем hello.asm и откроем этот файл с помощью текстового редактора: (рис.2 [-@fig:001]).

![рис 2](image/2.png){#fig:001 width=70%}

3. Скомпилируем данный текст,после проверим, что объектный файл был создан: (рис.3 [-@fig:001]).

![рис 3](image/3.png){#fig:001 width=70%}

4. Скомпилируем исходный файл hello.asm в obj.o и создадим файл листинга list.lst (рис.4 [-@fig:001]).

![рис 4](image/4.png){#fig:001 width=70%}

5. Передадим объектный файл на обработку компоновщику и проверим, что исполняемый файл hello был создан (рис.5 [-@fig:001]).

![рис 5](image/5.png){#fig:001 width=70%}

6. Запустим на выполнение созданный исполняемый файл, находящийся в текущем каталоге  (рис.6 [-@fig:001]).

![рис 6](image/6.png){#fig:001 width=70%}

7. Внесём изменения в текст программы (рис.7 [-@fig:001]).

![рис 7](image/7.png){#fig:001 width=70%}

8. Оттранслируем полученный текст программы lab5.asm в объектный файл. Выполним компоновку объектного файла и запустим получившийся исполняемый файл (рис.8 [-@fig:001]).

![8](image/8.png){#fig:001 width=70%}

![8.2](image/8.2.png){#fig:001 width=70%}

9. Скопируем файлы hello.asm и lab5.asm в локальный репозиторий и загрузим файлы на Github  ([-@fig:001]).




# Выводы

В ходе выполнения работы, я освоила процедуры компиляции и сборки программ, написанных на ассемблере NASM.


