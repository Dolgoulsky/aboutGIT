# README.md в GITHUB
## Как правило, в README.md проекта можно найти следующую информацию:
1. Название проекта и его краткое описание: кем создан, для чего, какие решает задачи и закрывает проблемы.
2. Технологии, которые применяются в проекте.
3. Документация проекта - подробная инструкция о том, что представляет собой проект.
4. Планы проекта, если они есть.


## Шпаргалка по Git и GitHub
pwd -- ( от англ. *print working dir*) - покажи в какой папке Я. <br>
ls -- ( от англ. *list directory content*) - покажи файлы и папки в текущей директории. <br>
ls -a  -- покажи скрытые файлы и папки. <br>
cd -- ( от англ. *change directory*) - сменить директорию. <br>
cd  first-project  -- сменить директорию и перейти в папку first-project. Где first-project является названием папки.<br>


## Пошаговая инструкция Git
1. Скачиваем\запускае Git Bash.
2. $ cd ~ -- Выходим в домашнюю директорию. *cd - change directory* - сменить директорию.
3. $ cd desktop -- Входим в нужную директорию, мой случай.
4. $ mkdir myproject -- создаем папку, где myproject это имя файла.
5. $ touch new-file.txt -- создаем фаил, где new-file.txt имя файла.
6. $ git init -- инициализация папки для отслеживания.
### Создаем или изменяем фаил. Сохраняем изминения.
7. $ git status -- Проверяем, ослеживается фаил или нет. Если название файла красное, то не отслеживается.
8. $ git add . -- Подготавливаем фаил к сохранению.
### Проверяем через git status, если название файла становится зеленым, то все хорошо.
