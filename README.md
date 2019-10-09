### Как подгрузить изменения к только что сделанному коммиту
[Git Basics: Adding more changes to your last commit](https://medium.com/@igor_marques/git-basics-adding-more-changes-to-your-last-commit-1629344cb9a8)

|Команда|Описание|
|---|---|
|git add .|Добавить файлы<br>(Если нужно только отредактировать сообщение коммита, этот пункт можно пропустить)|
|git commit --amend --no-edit|Добавить к коммиту без изменения сообщения|
|git commit --amend -m 'Some msg'|Добавить к коммиту c изменением сообщения|
|git push|Если коммит еще не Запушен|
|git push -f|Если коммит еще уже Запушен|