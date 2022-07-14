# Инструкция о работе с Git 

## Создание нового репозитория

Чтобы создать новый репозиторий, нам нужно открыть терминал, зайти в папку нашего проекта и выполнить команду **init**.

* Команда __git init__

Это включит приложение в этой конкретной папке и создаст скрытую директорию *__.git__*, где будет храниться история репозитория и настройки.

В папке можно создать файл, он будет храниться в директории **.git**.


## Определение состояния

Команда, которая показывает информацию о текущем состоянии репозитория (актуальна ли информация на нём, нет ли чего-то нового, что поменялось, и так далее) - **status**.

* Команда **git status**

При использовании команды возможно выйдет сообщение о том, что файл, который был добавлен в папку, неотслеживаемый. Оно выглядит следущим образом:

![пример сообщения](1.jpg)


Это значит, что файл новый и система еще не знает, нужно ли следить за изменениями в файле или его можно просто игнорировать. Для того, чтобы начать отслеживать новый файл, нужно его специальным образом объявить.

## Подготовка файлов 

В git есть концепция области подготовленных файлов. Можно представить ее как холст, на который наносят изменения, которые нужны в коммите. Сперва он пустой, но затем мы добавляем на него файлы (или части файлов, или даже одиночные строчки) командой **add** и, наконец, коммитим все нужное в репозиторий (создаем слепок нужного нам состояния) командой **commit**.

* Команда __git add__
* Команда __git commit__

Команда позволяет добавить файл(файлы) к следующему коммиту. 


## Фиксация изменений 

Для сохранения изменений, их необходимо закоммитить. Но чтобы это сделать успешно, нужно обозначить эти файлы для Git командой __git add__. Эта команда готовит файлы к коммиту.

Добавлять их можно по отдельности, например: **git add file1, git add file2**.

А также вместе. Для этого нужно использовать команду **git add .** 

Для создания коммита используем команду **git commit -m**

Флажок -m задаст commit message - комментарий разработчика. Он необходим для описания закоммиченных изменений.


## Просмотр коммитов 



