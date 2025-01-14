# Инструкция по работе с git
![Официальный логотип git](logo.png)

## Lesson 1

## Что такое git и контроль версий
**Системы контроль версий** - это системы, которые: 
1. обеспечивают сохранение содержимого файлов и папок(их *версий*)
2. Обеспечивают передвижение по *версиям* этих файлов и папок

**git** - это самая известная и используемая на данный момент реализация контроля версий с командным интерфейсом

**Локальный репозиторий** - это хранилище *изменений* Git в виде папки.

## Инициализация локального репозитория

Для того чтобы сказать git, что данная папка является локальным репозиторием нужно зайти в папку и ввести в ней команду

*git init*

Также, если этого раньше не делалось, то нужно определить ваше имя пользователя и email командами:
. git config --global user.name "your name"
. git config --global user.email your email 

## Добавление файлов под контроль версий

Для этого нужно ввести команду:
*git add имена файлов*
Теперь имена и содержимое этих файлов можно сохронять

## Делаем коммит

Для того, чтобы изменения представляли собой отдельную версию, к которой можно возвращаться и манипулировать после добавления под **контроль версий**, нужно ввести команду:

*git commit -m "Название версии"*

Можно также добавить под контроль версий и сформировать коммит для всех  файлов и папок одной командой:
*git commit -am "Название версии"

## Просмотр текущего состояния репозитория
Для вывода текущего состояния локального репозитория используются команды:

>git status - просмотр состояния файлов и папок в репозитории

> git diff - просмотр самих изменений файлов и папок

## Просмотр всех изменений репозитория

Для просмотра истории изменений от начала и последнего коммита нужно ввести:

*git log*

git status - команда, вывод состояния репозитория
git init - иницыализация git
## Lesson 2
git branch - выводит ветки
branch
git branch name - создание ветки
Github




## Отправка изменений в удалённый репозиторий

Отправлять изменения в удалённый репозиторий можно параметром **push** с указанием имени репозитория и ветки.

> git push origin main

Эта команда передаёт локальные изменения в центральный репозиторий, где с ними могут ознакомиться другие участники проекта.

## Отправка новой ветки в удалённый репозиторий

Передать новую ветку в удалённый репозиторий можно параметром push с флагом **-u**, указав имя репозитория и имя ветки.

> git push -u origin new_branch

## Удаление удалённой ветки

Чтобы избавиться от удалённой ветки, используйте параметр **push** с флагом **--delete**, указав имя удалённого репозитория и имя ветки.

> git push --delete origin existing_branch

## Получение изменений из удалённого репозитория

Для загрузки изменений из удалённого репозитория используется параметр **pull**. Он скачивает копию текущей ветки с указанного удалённого репозитория и объединяет её с локальной копией.

> git pull

Также можно просмотреть подробные сведения о загруженных файлах с помощью флага **--verbose**.

> git pull --verbose

## Слияние удалённого репозитория с локальным

Слияние удалённого репозитория с локальным выполняется параметром merge с указанием имени удалённого репозитория.

> git merge origin

## Удаление удалённой ветки

Чтобы избавиться от удалённой ветки, используйте параметр **push** с флагом **--delete**, указав имя удалённого репозитория и имя ветки.

> git push --delete origin existing_branch