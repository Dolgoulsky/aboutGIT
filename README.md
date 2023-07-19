# README.md в GITHUB
## Как правило, в README.md проекта можно найти следующую информацию:
1. Название проекта и его краткое описание: кем создан, для чего, какие решает задачи и закрывает проблемы.
2. Технологии, которые применяются в проекте.
3. Документация проекта - подробная инструкция о том, что представляет собой проект.
4. Планы проекта, если они есть.


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
9. $ git push -u origin main -- Дальше команда идет без ключа -u



## Шпаргалка по Git и GitHub
pwd -- ( от англ. *print working dir*) - покажи в какой папке Я. <br>
ls -- ( от англ. *list directory content*) - покажи файлы и папки в текущей директории. <br>
ls -a  -- покажи скрытые файлы и папки. <br>
cd -- ( от англ. *change directory*) - сменить директорию. <br>
cd ~ -- перейти в домашнюю директорию. <br>
cd.. -- перейти на уровень выше.<br>
cd/ -- Перейти в корневую директорию. <br>
cd  first-project  -- сменить директорию и перейти в папку first-project. Где first-project является названием папки.<br>
cd  first-project/html -- Перейти в first-project, в папку .html <br>


### Работа с файлами и папками.
$ touch index.html -- создать фаил index.html в текущей папке. <br>
$ touch index.html style.css script.js -- если нужно создать сразу несколько файлов, можно напечать их одной строкой, через пробел.<br>
$ mkdir (от англ. *make directory*) создать директорию в текущей папке. <br>


### Копирование и перемещение файлов.
$ cp file.txt ~/ -- (cp - *copy*) скопируй файл в другое место. <br>
$ mv file.txt ~/my dir -- ( англ. *move* - переместить) переместить фаил или папку в другое место.<br>


### Чтение фаилов.
$ cat file.txt (англ. *concatinate and print*) обьеденить и распечатать.<br>

### Удаление файлов и папок.
$ rm about.html -- (англ. *remove*) удалить фаил. Где about.html это название файла.<br>
$ rmdir images -- (англ. *remove directory*) удалить папку. Где images это название папки. <br>
$ rm -r second-project -- (англ. *remove + recursive) удалить папку и все что она содержит. <br>


### Инициализация репозитария.
$ git init - (англ. *initialize*) Чтобы Git отслеживался изменения в проекте, папку с файлами этого проекта, этого проекта, нужно сделать Git- репозитарием.<br>


### Разгитить папку
-- Для этого нужно удалить скрытую папку .git
$ cd name fail
$ rm -rf.git -- Ключ -R, позволяет удалить папку вместе с содержимым. Ключ -F (force -заставить) избавляет от лишних вопросов системы.<br>


### Git status
-- Проверить в каком статусе находится фаил.


### Git add - подготовка файла к сохранению.
$  git add text.txt -- Подготовка к сохранению одного, конкретного файла.
$  git add. - Не сохраняет фаил, только запоминает текущие соодержимое файла. 


### Git commit
$ git commit -m -- Ключ -М, позволяют присвоить коммиту сообщение. Такие сообщение должны быть информативными и четко описывать изменения. <br>


### Git commit - История коммитов.



### Создаем удаленный репозитарий.
-- Заходим в Github, ищем зеленую кнопку  *New*. Даем имя и жмем на зеленую кнопку *Create repository*. <br>

### SSH - Secure Shell Protocol.
$ cd ~/.ssh
$ ls  -- Ищите файлы  *id_dsa* или *id_rsa* и соответствующий ему фаил с расширением *.pub*! Фаил с расширением .pub - это ваш открытый ключ, а второй фаил, это ваш секретный ключ.<br>
$ ssh-keygen -t ed25519-c extremetechnology@mail.ru или 
$ ssh-keygen -t rsa -b 4096 -c extremetechnology@mail.ru - Если все хорошо, то увидим сообщение?: - Generating public/private ed25519 key. <br>
-- Далее нажимаем ENTER и сохранением место для хранения ключей. Passphrase - кодовая фраза для доступа к ключу. Можно не вписывать и просто нажать дважды ENTER.<br>
$  cat ~/.ssh/id_rsa.pub -- вытащить публичный ключ. Еще вариант:<br>
$  cat ~/.ssh/id_ed255519.pub -- второй вариант.<br>


### Привязка SSH кляча к Github.
-- Скопируем содержимое файла с публичными ключами в буфер обмена.<br>
-- Переходим в Github/Setting -- В меню слева жмем на пункт SSH and GPC keys. <br>
-- Нажимаем на зеленую кнопку *New SSH key*<br>
-- В - Title - набираем Personal key. <br>
-- Key type - выбираем - Authentication -<br>
-- В поле Key  - скопируем ключ из буфера обмена.<br>
-- Если вы в первый раз используете Git, то получите сообщение что все ОК. <br>


### Убедитесь, что репозитарии связаны.
$ git remote -v (англ. *verbose - подробный*) -- Должны появится две строчки:<br>
origin  git@github.com:Dolgoulsky/aboutGIT.git (fetch)<br>
origin  git@github.com:Dolgoulsky/aboutGIT.git (push)<br>


### Head - всему голова.
$ git log -после выхова этой команды, можно увидеть надпись (HEAD->MASTER)
- Фаил HEAD (Голова) - один из служебных файлов папки .git Он указывает на коммит, который сделан последним.

### Статус файлов в GIT
- Одна из ключевых задач в GIT, отслеживать измение файорв в репозитарии. Статусы: 

- untracked (англ. неотслеживаемый) 
Git видит что фаил существует, но не следит за изменениями в нем. У untracked файла нет предыдущих версий, завиксированных в коммитах или через команду git add.

- stagen (англ. подготовленный)
После выполнения команды git add. фаил попадет в staging area, то есть в список файорв, котррые войдут в коммит. В этот момент файл находится в состоянии stage = сцена = этап. 

Пример: git add добавляет персонажи на сцену, для общей фотографии, a git commit делает снимок сцены целиком.

- tracked (англ. отслеживаемый)
Состояние tracker - это противоположенное, состоянию antracked. В него попадают файлы, которые были зафиксирова с помощью git commit, а также файлы которые были добавлены командой git add. 

- modified  (англ. измененый)
Состояние modified означает, что Git сравнил содержимое файлов с последней версией и нашел отличия.

### Жизненый цикл файла GIT
- Состояние - UNTRACKED. Фаил только что создан. Git про него еще нечего не знает. 
- Состояние TRACKED. Фаил добавлен staging area c помощью git add. 
- Большинство файлов в проектах шагает по следующиму циклу: Изменен - Добавлен в список на коммиты - Закомичен. 



### Conventional Commits
Предпологает такой формат коммита: <type>:<сообщение>
- feat (англ. навык) - для новых функций.
- fix (англ. исправить, устранить) - для исправления ошибок.
$ git coomit -m "Добавить подсчет суммы"

### Как сделать mermaid - схему.
HEAD -- это голова.
Коммит -- всему голова. 
<тут пустая строка!>

```mermaid
graph LR;
untracked -- git add --> staget;
staged -- git commit -m --> tracked/commited; 
%% стрелка без текста для примера:
A --> B;

```

### How to deploy(02)

```mermaid 
graph TD;
A-->B;
A-->C;
B-->D;
C-->D;
```


### How to deploy (03)

```mermaid
flowchart TD
    A[Deploy to prodaction] --> B{Is it Friday};
    B -- Yes --> C[Do not deploy!];
    B -- No --> D[Run deploy.sh to deploy!];
    C ----> E[Enjoy your weekend];
    D ----> E[Enjoy your weekend];
```


### Как исправить коммит
- amend (англ. исправить ил дополнить) команда работает только с последним коммитом (HEAD)
- no-edit. Она сообщет команде commit, что нужно сотавить как было.
$ git commit --amend --no-edit

-m "Изменить сообщение последнего коммита"
$ git commit --amend -m "Изменить сообщение последнего коммита"


### Как откатить назад если все сломалось.
$ git restore -- staged <file> - переведет фаил из STAGED обратно в MODIFIED или UNTRACKED
$ git reset -- hard <commit hash> - откатит историю до коммита с хешем <Hash>. Более позние коммиты потеряются. 
- $ git log --online # ищем хешь для удаления.
7b972f5
b576d89 
$ 










