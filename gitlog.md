[< к Cодержанию>](./readme.md)

Научимся просматривать историю проекта.
Получение списка произведенных изменений — функция команды 
> git log

В результате увидим список коммитов в репозиторий, которые мы успели совершить.

+ Однострочная история
> git log --pretty=oneline

+ Контроль отображения записей
> git log --pretty=oneline --max-count=2  
> git log --pretty=oneline --since='5 minutes ago'  
> git log --pretty=oneline --until='5 minutes ago'  
> git log --pretty=oneline --author=<your name>  
> git log --pretty=oneline --all

+ Изменяем конечный формат лога

> git log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short

Давайте рассмотрим его в деталях:

+ --pretty="..." — определяет формат вывода.
- %h — укороченный хэш коммита
- %d — дополнения коммита («головы» веток или теги)
- %ad — дата коммита
- %s — комментарий
- %an — имя автора
- --graph — отображает дерево коммитов в виде ASCII-графика
- --date=short — сохраняет формат даты коротким и симпатичным


***

### ***Следующий шаг [git log](./gitlog.md)***