---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Архитектура компьютера"
author: "Сахно Никита НКАбд05-23"
 
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
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
 
# Цель работы
 
Целью работы является освоение процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.
 
# Задание
 
В соответствующем каталоге сделайте отчёт по лабораторной работе No 2 в формате
Markdown. В качестве отчёта необходимо предоставить отчёты в 3 форматах: pdf, docx
и md.
Загрузите файлы на github.
 
# Выполнение лабораторной работы
 
1. Я скачал Tex Live и Pandoc с официального сайта, через консоль и затем зашел в консоль (cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc/) в каталог, сформированный во время lab02 (Рис. 1)
 
![Рис. 1](study_2023-2024_arh-pc/labs/lab03/report/image/рис1.jpg){#fig:001 width=70%}
 
Я обновил локальный репозиторий, скачав изменения из удаленного репозитория с помо-
щью команды git pull (Рис. 2)
 
![Рис. 2](study_2023-2024_arh-pc/labs/lab03/report/image/рис2.jpg){#fig:001 width=70%}
 
Далее я провел компиляцию шаблона с использованием Makefile с помощью команды "make"
При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx.
Откройте и проверьте корректность полученных файлов. (Рис. 2)
 
![Рис. 3](study_2023-2024_arh-pc/labs/lab03/report/image/рис3.jpg){#fig:001 width=70%}
 
Удалил полученные файлы с использованием Makefile. Для этого ввел команду make clean (Рис. 4)
![Рис. 4](study_2023-2024_arh-pc/labs/lab03/report/image/рис4.jpg){#fig:001 width=70%}
 
Я открыл файл  report.md c помощью текстового редактора gedit gedit report.md (Рис. 5 и Рис. 6)
 
![Рис. 5](study_2023-2024_arh-pc/labs/lab03/report/image/рис5.jpg){#fig:001 width=70%}
 
![Рис. 6](study_2023-2024_arh-pc/labs/lab03/report/image/рис6.jpg){#fig:001 width=70%}
 
Далее я заполнил отчет и выгрузил его на гитхаб командами:
cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc
git add .
git commit -am 'feat(main): add files lab-3'
git push
(Рис. 7 и Рис. 8)
 
![Рис. 7](study_2023-2024_arh-pc/labs/lab03/report/image/рис7.jpg){#fig:001 width=70%}
 
![Рис. 8](study_2023-2024_arh-pc/labs/lab03/report/image/рис8.jpg){#fig:001 width=70%}
 
# Выводы
 
Я освоил процедуры оформления отчетов с помощью легковесного языка разметки markdown
 
# Список литературы{.unnumbered}
1. GDB: The GNU Project Debugger. — URL: https://www.gnu.org/software/gdb/.
2. GNU Bash Manual. — 2016. — URL: https://www.gnu.org/software/bash/manual/.
3. Midnight Commander Development Center. — 2021. — URL: https://midnight-commander.
org/.
4. NASM Assembly Language Tutorials. — 2021. — URL: https://asmtutor.com/.
5. Newham C. Learning the bash Shell: Unix Shell Programming. — O’Reilly Media, 2005. —
354 с. — (In a Nutshell). — ISBN 0596009658. — URL: http://www.amazon.com/Learning-
bash-Shell-Programming-Nutshell/dp/0596009658.
6. Robbins A. Bash Pocket Reference. — O’Reilly Media, 2016. — 156 с. — ISBN 978-1491941591.
7. The NASM documentation. — 2021. — URL: https://www.nasm.us/docs.php.
8. Zarrelli G. Mastering Bash. — Packt Publishing, 2017. — 502 с. — ISBN 9781784396879.
9. Колдаев В. Д., Лупин С. А. Архитектура ЭВМ. — М. : Форум, 2018.
10. Куляс О. Л., Никитин К. А. Курс программирования на ASSEMBLER. — М. : Солон-Пресс,
2017.
11. Новожилов О. П. Архитектура ЭВМ и систем. — М. : Юрайт, 2016.
12. Расширенный ассемблер: NASM. — 2021. — URL: https://www.opennet.ru/docs/RUS/nasm/.
13. Робачевский А., Немнюгин С., Стесик О. Операционная система UNIX. — 2-е изд. — БХВ-
Петербург, 2010. — 656 с. — ISBN 978-5-94157-538-1.
14. Столяров А. Программирование на языке ассемблера NASM для ОС Unix. — 2-е изд. —
М. : МАКС Пресс, 2011. — URL: http://www.stolyarov.info/books/asm_unix.
15. Таненбаум Э. Архитектура компьютера. — 6-е изд. — СПб. : Питер, 2013. — 874 с. —
(Классика Computer Science).
16. Таненбаум Э., Бос Х. Современные операционные системы. — 4-е изд. — СПб. : Питер,
2015. — 1120 с. — (Классика Computer Science)
