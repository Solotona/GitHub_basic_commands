# github_Homework_2

| № | Question | Answer |
|---|:---------|:-------|
| 1 | На локальном репозитории сделать ветки для: <br>*Postman*<br>*Jmeter*<br>*CheckLists*<br>*Bug_Reports*<br>*SQL*<br>*Charles*<br>*Mobile_testing*| `git branch`     |
| 2 | Запушить все ветки на внешний репозиторий        | `git push -u origin Postman`<br>[▷ Read about](#git-push)      |
| 3 | В ветке *Bug_Reports* сделать текстовый документ со структурой баг репорта        | `git checkout Bug_report && cat > Bug_Report.txt`      |
| 4 | В ветке *Bug_Reports* сделать текстовый документ со структурой баг репорта        | `git add .`<br>`git commit -m "comment"`<br>`git push -u origin Bug_report`     |
| 5 | Вмержить ветку *Bag Reports* в *Main*        | `git checkout main`<br>`git merge Bug_Report`    |
| 6 | Запушить *Main* на внешний репозиторий        | `git push -u origin applePay`<br>Затем во внешнем репозитории идем в альтернативную ветку и делаем Pull Request, чтобы смержить альтернативную ветку с main|
| 7 | В ветке *CheckLists* набросать структуру чек листа       |  `git checkout CheckLists`<br>`cat > Checklist.txt`<br>1 Список   проверок<br>2 Статус    |
| 8 | Запушить структуру на внешний репозиторий       | `git add Checklist.txt`<br>`git commit -m “Checklist.txt”`|
| 9 | На внешнем репозитории сделать Pull Request ветки *CheckLists* в *Main*       |  **На github идем в альтернативную ветку и делаем Pull Request, чтобы смержить альтернативную ветку с main**    |
| 10 | Синхронизировать Внешнюю и Локальную ветки *Main*       | `git checkout main<br>git fetch<br>git pull`     |

## **==== Описание команд =====**
### git push
позволяет отправлять локальную ветку на удаленный репозиторий. Она помогает разработчикам синхронизироваться в команде, а именно отправляет проделанные изменения. Если программист работает один, то пуш позволяет хранить код в облаке, например github, gitlab и не только, избавляя от риска потери данных на компьютере.

Выполнив команду **git push -u origin master** вы устанавливаете связь между той веткой, в которой вы находитесь и веткой master на удалённом сервере. Команду требуется выполнить единожды, чтобы потом можно было отправлять/принимать изменения лишь выполняя git push из ветки, без указания всяких алиасов для сервера и удалённых веток. Это сделано для удобства.


### git branch
позволяет создавать, просматривать, переименовывать и удалять ветки. Она не дает возможности переключаться между ветками или выполнять слияние разветвленной истории. Именно поэтому команда git branch тесно связана с командами git checkout и git merge.


### git checkout
позволяет перемещаться между ветками, созданными командой git branch. При переключении ветки происходит обновление файлов в рабочем каталоге в соответствии с версией, хранящейся в этой ветке, а Git начинает записывать все новые коммиты в этой ветке.

**параметр -b** — это удобный способ сообщить системе Git, чтобы она выполнила команду `git branch <новая-ветка>` перед выполнением команды `git checkout <новая-ветка>` . По умолчанию команда `git checkout -b` создает новую ветку от текущего указателя HEAD.


### git merge
объединяет несколько последовательностей коммитов в общую историю. Чаще всего команду git merge используют для объединения двух веток.
Git merge название ветки, которую мержишь (в начале становишься куда мержишь).


### git fetch
команда в распределенной системе контроля версий Git, которая используется для скачивания изменений из удаленного или локального репозитория в свой локальный репозиторий. Польза git fetch в том, что эта команда привносит актуальность локальному репозиторию без изменения его дерева или текущей ветки.


### git pull 
используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым.

### Файл .gitignore
нужен для скрытия файлов и папок от системы контроля версий Git. Обычно скрывают конфигурационные файлы (особенно с паролями), временные файли и папки.

### Операции отмены git restore и git reset
Отмена может потребоваться, если вы сделали коммит слишком рано, например, забыв добавить какие-то файлы или комментарий к коммиту. Если вы хотите переделать коммит — внесите необходимые изменения, добавьте их в индекс и сделайте коммит ещё раз, указав параметр --amend:
`$ git commit --amend`
Эта команда использует область подготовки (индекс) для внесения правок в коммит. Если вы ничего не меняли с момента последнего коммита (например, команда запущена сразу после предыдущего коммита), то снимок состояния останется в точности таким же, а всё что вы сможете изменить — это ваше сообщение к коммиту.

Запустится тот же редактор, только он уже будет содержать сообщение предыдущего коммита. Вы можете редактировать сообщение как обычно, однако, оно заменит сообщение предыдущего коммита.

Например, если вы сделали коммит и поняли, что забыли проиндексировать изменения в файле, который хотели добавить в коммит, то можно сделать следующее:

`$ git commit -m 'Initial commit'
$ git add forgotten_file
$ git commit --amend`
В итоге получится единый коммит — второй коммит заменит результаты первого.

Примечание: Очень важно понимать, что когда вы вносите правки в последний коммит, вы не столько исправляете его, сколько заменяете новым, который полностью его перезаписывает. В результате всё выглядит так, будто первоначальный коммит никогда не существовал, а так же он больше не появится в истории вашего репозитория.

Очевидно, смысл изменения коммитов в добавлении незначительных правок в последние коммиты и, при этом, в избежании засорения истории сообщениями вида «Ой, забыл добавить файл» или «Исправление грамматической ошибки»

### Git restore staged
это команда в Git, которая позволяет вернуть файлы в состояние до добавления их в индекс. Она может быть полезна, когда нужно отменить добавление файлов в индекс, чтобы потом изменения были сохранены другим способом. Git версии 2.23.0 представил новую команду: `git restore`. Начиная с версии 2.23.0, Git будет использовать git restore вместо git reset для многих операций отмены.
Откат изменённого файла с помощью git restore
Что, если вы поймете, что не хотите сохранять изменения в файле CONTRIBUTING.md? Как легко его откатить — вернуть обратно к тому, как он выглядел при последнем коммите (или изначально клонирован, или каким-либо образом помещён в рабочий каталог)? К счастью, git status тоже говорит, как это сделать. В выводе последнего примера, неиндексированная область выглядит следующим образом:

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   CONTRIBUTING.md
Он довольно недвусмысленно говорит, как отменить сделанные вами изменения. Давайте сделаем то, что написано:

$ git restore CONTRIBUTING.md
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	renamed:    README.md -> README
Важно
Важно понимать, что git restore <file> — опасная команда. Любые локальные изменения, внесённые в этот файл, исчезнут — Git просто заменит файл последней зафиксированной версией. Никогда не используйте эту команду, если точно не знаете, нужны ли вам эти несохранённые локальные изменения.


Как удалить локальный репозиторий

Как удалить удаленный репозиторий

Как создать пустой репозиторий, а потом ветки


## **=====Лекция=====**

Пишем git branch и видим ветки (например, main).
Пишем git branch applePay и смотрим через git branch, видим что появилась ветка applePay. Так мы просто создали ветку.
Если мы хотим создать ветку и в нее перейти, то используем команду git checkout -b sumsungPay


Переходим в главную ветку git checkout main
Чтобы свичнутся (перейти) в нужную папку указываем название git checkout applePay
Открываем папку, чтобы посмотреть start .. в графическом интерфейсе

Создаем  файлик cat > transact.json (видим, что в текущей папке появился файл).
git add .
git commit -m “transact.json” (без пуша пока).

git checkout main - переходим в главную ветку и файл transact не отражается
git checkout applePay - снова переходим в альтернативную ветку и файл transact.json появляется. В этом смысл git, работа на альтернативных ветках, пока не будет принудительного смерживания с основной веткой.

Если мы хотим вмержить в основную ветку, чтобы файл transact.json появился в ветке main. В начале переходим в целевую ветку, в которую будем заливать файл - git checkout main, затем через команду git merge пишем название ветку, которую нужно вкатить: git merge applePay. Теперь мы видим, что файл есть на ветке main и applePay.

Теперь посмотрим, как резолвить конфликт.
Переходим в альтернативную ветку checkout applePay и редактируем файл nano transact.json. Коммитим изменения git commit -a -m “transact.json 2 version”
Возвращаемся в основную ветку git checkout main.
git merge applePay и видим сообщение о конфликте (Automatic merge failed; fix conflicts and then commit the result). Чтобы пофиксить конфликт, открываем файл cat transact.json и начинаем редактировать, как нам нужно, чтобы зарезолвить конфликт.

Ветки applePay и samsungPay находится пока только на локальном репозитории. Переходим на внешний репозиторий.
git push -u origin applePay.

Затем во внешнем репозитории идем в альтернативную ветку и делаем Pull Request, чтобы смержить main и ветку applePay.

Чтобы изменения отразились локально, идем в главную ветку - checkout main, проверяем, что нет файла ls -la. Делаем git fetch, чтобы проверить, что да, есть изменения. И git pull
