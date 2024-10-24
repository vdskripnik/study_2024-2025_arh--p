---
## Front matter
title: "Лабораторная работа №3"
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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.

# Задание

1. В соответствующем каталоге сделайте отчёт по лабораторной работе № 2 в формате
Markdown. В качестве отчёта необходимо предоставить отчёты в 3 форматах: pdf, docx
и md.
2. Загрузите файлы на github.

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

Перехожу в каталог курса сформированный при выполнении лабораторной работы
№2. (рис.1.1 [-@fig:001]).

![рис.1.1](image/1.png){width=100%}

Обновляю локальный репозиторий, скачав изменения из удаленного репозитория.(рис.1.2 [-@fig:001]).

![рис.1.2](image/2.png){width=100%}

Перехожу в каталог с шаблоном отчета по лабораторной работе № 3.Провожу компиляцию шаблона с использованием Makefile. Для этого ввожу команду make.(рис.1.3 [-@fig:001]).

![рис.1.3](image/3.png){width=100%}

При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx.
Открываю и проверяю корректность полученных файлов.(рис.1.4 [-@fig:001]).

![рис.1.4](image/4.png){width=100%}

Удаляю полученный файлы с использованием Makefile. Для этого ввожу команду make clean.(рис.1.5 [-@fig:001]).

![рис.1.5](image/5.png){width=100%}

Открываю файл report.md c помощью любого текстового редактора, например gedit gedit report.md.(рис.1.6 [-@fig:001]).

![рис.1.6](image/6.png){width=100%}

Заполняю отчет.(рис.1.7[-@fig:001]).

![рис.1.7](image/7.png){width=100%}

Загружаю файлы на Github.(рис.1.8[-@fig:001]).

![рис.1.8](image/8.png){width=100%}




# Выводы

В ходе работы я ознакомилась с тем, как в Markdown задается начертание шрифтов, оформляются изображения и ссылки на них.

# Список литературы{.unnumbered}

::: {#refs}
:::
