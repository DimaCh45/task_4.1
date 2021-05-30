[< к Cодержанию>](./readme.md)

+ Команда **git status** - проверка состояния репозитория

```
git status
```

Результат команды 

`git status
On branch master
nothing to commit (working directory clean) `

Команда проверки состояния сообщит, что коммитить нечего. Это означает, что в репозитории хранится текущее состояние рабочего каталога, и нет никаких изменений, ожидающих записи.

+ Откроем и изменим содержимое файла readme.md любым текстовым редактором

Проверим состояние 

```
git status
```

Результат команты
```
git status
# On branch master
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#   modified:   readme.md
#
no changes added to commit (use "git add" and/or "git commit -a")
```
Git знает, что файл readme.md был изменен, но при этом эти изменения еще не зафиксированы в репозитории.

Также обратите внимание на то, что сообщение о состоянии дает вам подсказку о том, что нужно делать дальше. Если вы хотите добавить эти изменения в репозиторий, используйте команду git add. В противном случае используйте команду git сheckout для отмены изменений.

Также просмотр изменений можно выполнить командой:

```
git diff
```
> git diff - Перечисляет все новые или изменённые файлы, которые нуждаются в фиксации

+ Введем команду

```
git add readme.md
```
Затем

```
git status
```
Мы увидим что измениния файла *readme.md* был проиндексирован.

+ Создаем комментарий

```
git commit -m "Update readme.md"
```


***

### ***Следующий шаг [gitignore](./gitignore.md)***
