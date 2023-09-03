# GITHub Homework 1

Для выполнения задания у вас должен быть установлен для Windows - Git Bash. Создан аккаунт в GitHub. Все шаги сценария выполняйте в терминале Git Bash, Terminal, в папке под гитом.

Как отправить ДЗ на проверку.
 1. Создайте текстовый файл, как в первом ДЗ по Terminal.
 2. Сценарий перенесите в этот файл.
 3. Напротив каждого действия - напишите команду в Git Bash
Файл со сценарием и ссылку на свой гит хаб.

## JSON 
| №  | Task  | Answer |
|:------------- |:---------------| :-------------|
| 4 | Создать внешний репозиторий c названием JSON.          | На сайте GitHub        |
| 5 | Клонировать репозиторий JSON на локальный компьютер          | `git clone` <br>вставляем сюда скопированную ссылку из  <>Code по протоколу https        |
| 6 | Внутри локального JSON создать файл “new.json”.          | `cat > new.json`        |
| 7 | Добавить файл под гит          | `git add new.json`        |
| 8 | Закоммитить файл          | `git commit -m "comments"`        |
| 9 | Отправить файл на внешний GitHub репозиторий          | `git push`        |
| 10 | Отредактировать содержимое файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.          | `nano new.json`<br>{<br>"name": "Natalia",<br>"lastName": "Tokareva",<br>"quantityPet": 1,<br>"salaryExpected": "500 USD"<br>}        |
| 11 | Отправить изменения на внешний репозиторий          | `git commit -a -m “new.json” && git push`        |
| 12 | Создать файл preferences.json          | `cat > preferences.json`        |
| 13 | В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON          | `nano preferences.json`<br>{<br>	"favoriteFilm": "Sea Inside",<br>	"favoriteSeries": "Friends",<br>	"favoriteFood": ["Khinkali", "Pho Bo", "soup", "pasta"],<br>	"favoriteSeason": ["spring", "summer"],<br>	"Country": "the USA"<br>}<br>Ctrl+O, Ctrl+X      |
| 14 | Создать файл skills.json добавить информацию о скиллах, которые будут изучены на курсе в формате JSON          | `cat > skills.json`<br> {<br>"Skills": ["API через Postman", "сниффинг http web трафика через Charles и Fiddler", "Dev Tools веб браузеров, командная строка", "основы SQL техники тест-дизайна"]<br>}     |
| 15 | Отправить сразу 2 файла на внешний репозиторий          | `git add ./`        |
| 16 | На веб интерфейсе создать файл bug_report.json          |         |
| 17 | Сделать Commit changes (сохранить) изменения на веб интерфейсе.          |        |
| 18 | На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.          | (See more...) [18]     |


 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 20. Синхронизировать внешний и локальный репозиторий JSON
git pull



XML
 21. Создать внешний репозиторий c названием XML.
 22. Клонировать репозиторий XML на локальный компьютер.
git clone

 23. Внутри локального XML создать файл “new.xml”.
cat > new.xml

 24. Добавить файл под гит.
git add new.xml

 25. Закоммитить файл.
git commit -m ‘добавлен новый файл’

 26. Отправить файл на внешний GitHub репозиторий.
git push

 27. Отредактировать содержимое файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
cat >> new.xml
<?xml version="1.0"?>
<CAT>
  <NAME>Natalia</NAME>
  <LASTNAME>Tokareva</BREED>
  <QUANTITYPET>1</QUANTITYPET>
  <SALARYEXPECTED>500 USD</SALARYEXPECTED>
</CAT>

 28. Отправить изменения на внешний репозиторий.
git add ‘new.xml’ | git commit -m ’new file’ | git push

 29. Создать файл preferences.xml
cat > preferences.xml

 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, страна которую хотели бы посетить) в формате XML.
cat >> preferences.xml
<?xml version="1.0"?>
<CAT>
  <FAVORITEFILM>Sea Inside</FAVORITEFILM>
  <FAVORITESERIES>Friends</FAVORITESERIES>
  <FAVORITEFOOD>Khinkali, Pho Bo soup, pasta,</FAVORITEFOOD>
  <FAVORITESEASON>spring, summer</FAVORITESEASON>
  <FAVORITECOUNTRY>USA</FAVORITECOUNTRY>
</CAT>

 31. Создать файл skills.xml добавить информацию о скиллах, которые будут изучены на курсе в формате XML
nano skills.xml
<?xml version="1.0" encoding="windows-1251">
<SKILLS>API через Postman, сниффинг http web трафика через Charles и Fiddler, Dev Tools веб браузеров, командная строка, основы SQL техники тест-дизайна</SKILLS>

 32. Сделать коммит в одну строку.
git add . && git commit -m "comment"

 33. Отправить сразу 2 файла на внешний репозиторий
git add ./

 34. На веб интерфейсе создать файл bug_report.xml
 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе

 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
<?xml version="1.0" encoding="windows-1251"?>
<root>
  <tree>
   	<ID>BR-1</ID>
   	<Summary>Кнопка Отправить не реагирует на клик на странице оформления заказа.</Summary>
   	<Project>www.test.pitomets.com</Project>
	<Version>5.1</Version>
	<Severity>Critical</Severity>
	<Priority>Middle</Priority>
	<Status>Open</Status>
	<Author>Tokareva Natalia</Author>
	<AssignedTo>Lead Developer</AssignedTo>
	<Description>
		<Precondition>
			<1>Зайти на сайт www.test.pitomets.com</1>
			<2>Перейти на страницу Питомцы</2>
		</Precondition>
		<Environment>Windows 11 Pro, Google Chrome v: 94.0.4606.71 (x86_64)</Environment>
		<Steps_to_reproduce>
			<1>Кликнуть на кнопку Оформить заказ в карточке питомца</1>
			<2>Заполнить поле Имя</2>
			<3>Заполнить поле телефон</3>
			<4>Заполнить поле E-mail</4>
			<5>Нажать кнопку Отправить</5>
		<Steps_to_reproduce>
        <Actual_result>Кнопка “Отправить” в форме заказа питомца не реагирует на клик.</Actual_result>
		<Expected_result>Пользователь перенаправляется на страницу подтверждения заказа. Есть сообщение, что заказ №#### отправлен, менеджер с вами свяжется в ближайшее время.</Expected_result>
	</Description>
	<Attachmen>https://drive.google.com/...</Attachmen>
  </tree>
</root>

 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 38. Синхронизировать внешний и локальный репозиторий XML
git pull


TXT
 1. Создать внешний репозиторий c названием TXT.  
На сайте GitHub создаем новый репозиторий через New - Create Repository. 

 2. Клонировать репозиторий TXT на локальный компьютер. 
Копируем URL в <>Code по HTTPS протоколу. Заходим через консоль GitBash в локальную папку: cd “g:/My Drive/QA/Ksendzov_Cours/git_intro”.
git clone https://github.com/Solotona/TXT.git

 3. Внутри локального TXT создать файл “new.txt”
nano new.txt (Ctrl+O - сохранение, Ctrl+X - выход)

 4. Добавить файл под гит.
git add new.txt

 5. Закоммитить файл.
git commit -m “comment”

 6. Отправить файл на внешний GitHub репозиторий.
git push

 7. Отредактировать содержимое файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.
cat >> new.json
Name: Natalia,
Last Name: Tokareva,
Quantity of Pet: 1,
Salary Expected: 500 USD.

 8. Отправить изменения на внешний репозиторий. 
git push

 9. Создать файл preferences.txt
nano preferences.txt

 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT.
nano preferences.txt
Favorite Film: "Sea Inside",
FavoriteSeries: "Friends",
Favorite Food: Khinkali, Pho Bo soup, pasta,
Favorite Season: spring, summer,
Country: the USA.

 11. Создать файл skills.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT.
nano skills.txt
Skills: тестирование API через Postman, сниффинг http web трафика через Charles и Fiddler, Dev Tools веб браузеров, командная строка, основы SQL техники тест-дизайна.

 12. Сделать коммит в одну строку.
git add . && git commit -m "comment"

 13. Отправить сразу 2 файла на внешний репозиторий.
git push

 14. На веб интерфейсе создать файл bug_report.txt.
 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT.
id: BR-1,
Summary: Кнопка Отправить не реагирует на клик на странице оформления заказа.,
Project: www.test.pitomets.com,
Version: 5.1,
Severity: Critical,
Priority: Middle,
	Status: Open,
	Author: Tokareva Natalia,
	Assigned To: Lead Developer,
	Description: 
		Precondition: 
			1: Зайти на сайт www.test.pitomets.com,
			2: Перейти на страницу Питомцы
		Environment: Windows 11 Pro, Google Chrome v: 94.0.4606.71 (x86_64),
		Steps to reproduce: 
			1: Кликнуть на кнопку Оформить заказ в карточке питомца,
			2: Заполнить поле Имя,
			3: Заполнить поле телефон,
			4: Заполнить поле E-mail,
			5: Нажать кнопку Отправить
		Actual result: Кнопка “Отправить” в форме заказа питомца не реагирует на клик.,
		Expected result: Пользователь перенаправляется на страницу подтверждения заказа. Есть сообщение, что заказ №#### отправлен, менеджер с вами свяжется в ближайшее время
Attachment: https://drive.google.com/...

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.


 18. Синхронизировать внешний и локальный репозиторий TXT
git pull


## 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
{<br>
	"id": "BR-1",<br>
	"Summary": "Кнопка Отправить не реагирует на клик на странице оформления заказа.",<br>
	"Project": "www.test.pitomets.com",<br>
	"Version": "5.1",<br>
	"Severity": "Critical",<br>
	"Priority": "Middle",<br>
	"Status": "Open",<br>
	"Author": "Tokareva Natalia",<br>
	"Assigned To": "Lead Developer",<br>
	"Description": {<br>
		"Precondition": {<br>
			"1": "Зайти на сайт www.test.pitomets.com",<br>
			"2": "Перейти на страницу Питомцы"<br>
		},<br>
		"Environment": "Windows 11 Pro, Google Chrome v: 94.0.4606.71 (x86_64)",<br>
		"Steps to reproduce": {<br>
			"1": "Кликнуть на кнопку Оформить заказ в карточке питомца",<br>
			"2": "Заполнить поле Имя",<br>
			"3": "Заполнить поле телефон",<br>
			"4": "Заполнить поле E-mail",<br>
			"5": "Нажать кнопку Отправить"<br>
		},<br>
		"Actual result": "Кнопка “Отправить” в форме заказа питомца не реагирует на клик.",<br>
		"Expected result": "Пользователь перенаправляется на страницу подтверждения заказа. Есть сообщение, что заказ №#### отправлен, менеджер с вами свяжется в ближайшее время"<br>
	},<br>
	"Attachment": "https://d rive.google.com/..."<br>
}<br>

Из курса Ксендзова Вадима:
Рекомендует создавать репозитории прямо на сайте GitHub. 
Заходим на главную страницу в виде дашборда. Слева меню - New Repositories - Называем.
Затем после создания копирует его на локальный компьютер: 
в репозитории кликаем на <>Code
копируем ссылку (протокол https)
В терминале создаем папку для гита:
git clone сюда_ссылка (Появляется папка гита)
Переходим в нее через cd, например, в Terminal (Появляется в скобочках (main)
Можем создать внутри файлик: cat > names.txt
Проверяем статус: git status (Сообщение On branch main означает, что находимся на главной ветке. Untracked files (есть неотслеживаемые файлы, т.е. на локальном компьютере есть изменения, как раз-таки чем занимается гит - отслеживанием истории версий). Есть подсказка Use  “git add <file>...” файлы подсвечены красным
git add names.txt (набрасываем файлы, которые пойдут потом в коммит)
git status (файлы стали подсвечены зеленым цветом)
git commit -m “names” - Команда commit - это точка сохранения, это фотография момента, в данном случае версии документа. После -m “” пишутся комментарии, что содержит этот коммит.
Забыли настроить git, чтобы не ругался. Устанавливаем имя и почту:
git config --global user.email "solotona@mail.ru"
git config --global user.name "Natalia"
git color.ui -  автоматически раскрасит большую часть своего вывода, если вы его об этом попросите. Вы можете очень тонко задать, что вы хотите раскрасить и как. Но, чтобы просто включить весь предустановленный цветной вывод для терминала, установите color.ui в true: $ git config --global color.ui true
Еще раз меняем файл: $ cat >> names.txt
Смотрим git status
Коммитим изменения: git commit -a -m “пишем комментарий” (опция -a означает git add, для краткости, если файл раньше уже был закоммитен, т.е. сейчас его просто модифицировали)
Затем опять git push.
Проверяем на внешнем репозитории обновление (на сайте github)
- - - - - - - - - - 
git add . - добавить все файлы

Работа в редакторе nano:
Ctrl+O - сохранить изменения
Ctrl+X - выйти
горячие клавиши:
Alt + Backspace поможет удалить слово, стоящее перед курсором (слева).
Ctrl + D удаляет все символы, которые находится справа от курсора в текущей строке.


Из курса ТГУ:

Вы можете получать доступ к данным в репозиториях и записывать их в GitHub.com с помощью SSH (протокол Secure Shell). При подключении через SSH проверка подлинности выполняется с помощью файла закрытого ключа на локальном компьютере. С помощью протокола SSH можно подключаться и проходить проверку подлинности на удаленных серверах и службах. 
С помощью ключей SSH вы можете подключаться к GitHub без указания имени пользователя и personal access token при каждом посещении. Вы также можете использовать ключ SSH для подписывания фиксаций.

Пошаговое создание репозитория на github: https://docs.github.com/ru/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Откройте GIT Bash
Вставьте приведенный ниже текст, указав свой адрес электронной почты GitHub:
$ ssh-keygen -t ed25519 -C "solotona@mail.ru" - генерация нового ключа SSH ed25519 на Linux. 
При появлении запроса "Ввести файл, в котором нужно сохранить ключ" (> Enter a file in which to save the key (/c/Users/YOU/.ssh/id_ALGORITHM):[Press enter]), можно нажать клавишу ВВОД , чтобы принять расположение файла по умолчанию. Обратите внимание, что если вы создали ключи SSH ранее, ssh-keygen может попросить вас переписать другой ключ. В этом случае рекомендуется создать ключ SSH с пользовательским именем. Для этого введите расположение файла по умолчанию и замените id_ssh_keyname именем пользовательского ключа.
Добавление ключа SSH в ssh-agent:
$ eval  "$(ssh-agent -s)" - убедитесь, что ssh-agent запущен
Добавьте закрытый ключ SSH в ssh-agent. Если вы создали ключ с другим именем или добавляете существующий ключ с другим именем, замените id_ed25519 в команде на имя файла закрытого ключа:
$ ssh-add ~/.ssh/id_ed25519
Добавьте открытый ключ SSH в учетную запись в GitHub:
cat ~/.ssh/id_ed25519.pub - выводим ключ этой командой, копируем и вставляем на сайте в личном кабинете. Setting -> SSH & GPG keys

Команды git:
git init "G:/My Drive/QA/git" - создать новый репозиторий Git (на курсе Вадим Ксендзов осознанно остерегает пользоваться этой командой, а лучше через интерфейс гитхаба)
cd "G:/My Drive/QA/git" - переходим в вновь созданную папку
echo 'Privet' > readme.md - создаем файл
git add readme.md - следуем реклмендациям 
git status - отображает состояние рабочего каталога и раздела проиндексированных файлов
git commit -m “”
Создаем репозиторий на странице github и добавляем несколько файлов:
git add .

git remote add origin git@github.com:solotona/git
git push -u origin main

git log -p покажет историю коммитов
