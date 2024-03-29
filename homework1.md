# Подсказка по GIT

## Инициализация пустого репозитория: изменение заголовка для создания конфликта
```sh
git init
```
Эта команда создаёт в текущем каталоге новый подкаталог с именем .git, содержащий все необходимые файлы репозитория — **структуру Git репозитория**.
***
## Добавить файл к отслеживанию:
```sh
git add
```
Добавление измененных файлов в индекс. После того, как все нужные файлы будут добавлены в индекс, можно будет из этих изменений сформировать коммит
***
## Добавить коммит:
```sh
git commit -m "Message"
```
Commit/Коммит - это способ **сохранения изменений** в коде. Каждый commit содержит информацию о том, что было изменено в коде и кем были внесены эти изменения. Они позволяют разработчикам **отслеживать** изменения в своем (или чужом) коде и **возвращаться** к предыдущим версиям, если это необходимо.
***
## Просмотр истории коммитов
```sh
git log
```
После того, как вы создали несколько коммитов или же клонировали репозиторий с уже существующей историей коммитов, вероятно вам понадобится возможность посмотреть что было сделано — **историю коммитов**.
***
## Просмотр истории коммитов в кратком виде:
```sh
git log --oneline
```
Вывод коммитов в одну строку. Показывает только хэш коммита и commit message
***
## Переключение между версиями 
```sh
git checkout <идентификатор>
```
Команда позволяет перемещаться между сохранениями (версиями)
***
## Создание новой ветки 
```sh
git branch <имя_ветки>
```
C помощью этой команды можно добавлять новые ветки
***
## Переключение между ветками 
```sh
git checkout <имя_ветки>
```
Команда позволяет перемещаться между ветками
***
## Удаление ветки 
```sh
git branch -d <имя_ветки>
```
Команда позволяет удалить ветку
***
## Просмотреть лог с отображением веток
```sh
git log --graph
```
Команда позволяет визуализировать ветвления
***
## Слить ветки 
```sh
git merge <имя_ветки>
```
Команда используется для **объединения** изменений из одной ветки в другую. Она применяется для слияния изменений, которые были внесены в отдельной ветке, обычно для объединения фиксации ошибок или добавления функциональности в проект
***
## Клонирование удаленного репозитория на компьютер 
```sh
git clone <ссылка на удаленный репозиторий>
```
Git создает копию репозитория, который находится по ссылке (<ссылка на репозиторий>). Также можно указать название новой папки, в которую Git скопирует репозиторий (<название папки>). Если его не указать, папка будет называться так же, как и сам репозиторий.
***
## Добавление удаленного репозитория 
```sh
git remote add origin <url>
```
Команда применяется чтобы добавить удаленный репозиторий и присвоить ему название, которое используется для удобства как сокращение адреса
***
## Отправить изменения на удалененый репозиторий 
```sh
git push -u origin main
```
Это консольная команда, которая передаёт в удалённый репозиторий изменения, сделанные в локальном репозитории.
***
## Запрос изменений в репозитории с сервера
```sh
git pull 
```
Команда используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым. Слияние удаленных вышестоящих изменений в локальный репозиторий — это обычное дело в процессе совместной работы на основе Git.
***
## Вытолкнуть ветку на удаленный репозиторий 
```sh
git push --set-upstream origin <имя ветки>
```
Команда используется чтобы "вытолкнуть" только ветку на удаленный репозиторий
***