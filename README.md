### Новый репозиторий - создать и загрузить на локальный компьютер
Сперва создать репозиторий на [сайте](https://github.com/new)

Затем создать папку на компьютере, открыть там командную строку и выполнить команды:

|Команда|Описание|
|---|---|
|git init|Инициализировать репозиторий у себя в папке|
|git remote add origin https://github.com/sergx/test_git|Связать локальный репозиторий с удаленным|
|*git remote set-url origin https://github.com/sergx/nodejs-test*|*Если не то название ввел, то этой командой можно переназначить*|
|git pull origin master|Загрузить файлы репозитория на локальный компьютер|
|**После внесения изменения в файлы:**|
|git add .|Добавить все изменения для коммита|
|git commit -m 'init'|Инициализировать коммит|
|git push --set-upstream origin master|Загрузить коммит и указать ветку (последющие пуши можно будет совершать через *git push*)|

#### Загрузить на локальную машину актуальную версию, ПЕРЕЗАПИСАВ то, что есть локально
[https://stackoverflow.com/a/8888015/6928687](https://stackoverflow.com/a/8888015/6928687)

|Команда|Описание|
|---|---|
|git fetch --all|Просто загружает самую последнюю версию файлов, без попыток мерджить и пр.|
|git reset --hard origin/master|Заново устанавливает связь с бранчем|

### Подгрузить изменения к только что сделанному коммиту
[Git Basics: Adding more changes to your last commit](https://medium.com/@igor_marques/git-basics-adding-more-changes-to-your-last-commit-1629344cb9a8)

|Команда|Описание|
|---|---|
|git add .|Добавить файлы<br>(Если нужно только отредактировать сообщение коммита, этот пункт можно пропустить)|
|git commit --amend --no-edit|Добавить к коммиту без изменения сообщения|
|git commit --amend -m 'Some msg'|Добавить к коммиту c изменением сообщения|
|git push|Если коммит еще не запушен|
|git push -f|Если коммит еще уже запушен|