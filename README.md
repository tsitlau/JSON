# JSON
 1. Создать внешний репозиторий c названием JSON.
Открыть https://github.com. Залогиниться. Нажать кнопку New.
В поле Repository name ввести JSON, выбрать Public и Add a README file.
Нажать Create repository

 2. Клонировать репозиторий JSON на локальный компьютер.
Нажать Code, выбрать HTTPS, скопировать ссылку на репозиторий, в gitbash зайти в папку, где будет размещен репозиторий),
git clone https://github.com/lvnnew/JSON.git
cd JSON - в терминале перейти в папку JSON, в конце адреса расположения отображается main

 3. Внутри локального JSON создать файл “new.json”.
touch new.json

 4. Добавить файл под гит.
git status - new.json отображается красным (изменения в файле не отслеживаются)
git add new.json
git status - new.json отображается зеленым (изменения в файле отслеживаются)

 5. Закоммитить файл.
git commit -m "add new.json" - создает снимок текущего состояния файла с комментарием add new.json

 6. Отправить файл на внешний GitHub репозиторий.
git push

 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
vim new.json
insert
{
	"full_name":"Tatyana Tsitlau",
	"age":"33",
	"number_of_pets":"1",
	"desired_salary":"900$"
}
esc
:wq

 8. Отправить изменения на внешний репозиторий.
git add new.json
git commit -m "modified new.json"
git push

 9. Создать файл preferences.json
touch preferences.json

 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
vim preferences.json
insert
{
	"favorite_movie":"The_Shawshank_Redemption",
	"favorite_series":"The_Beauty_Inside",
	"favorite_food":"pizza",
	"favorite_time_of_year":"summer",
	"country_I_want_to_visit":"Japan"
}
esc
:wq

 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
cat > skills.json
"skills":[
	"software testing theory",
	"client-server architecture",
	"HTTP Server Request Methods",
	"HTTP server Response codes",
	"Structures of HTTP requests and responses",
	"What is JSON, XML. Their structure",
	"API testing via Postman JS, API autotests",
	"Removing and reading logs from an external server",
	"Sniffing http web traffic through Charles and Fiddler",
	"Dev Tools of web browsers Google Chrome, FireFox",
	"VPN. How it works, why you need it, how to use it, tool options",
	"Mobile testing",
	"Feature of iOS, Android, guidelines",
	"Build iOS applications on Xcode",
	"Build Android applications on Android Studio",
	"ADB management of android devices",
	"Setting up proxy and vpn on iOS and Android",
	"Interception (sniffing) of mobile traffic through Charles and Fiddler on iOS and Android",
	"Command line (terminal) Linux copy, create, view, move files on servers without a graphical interface",
	"Basics of bash scripting, automation of routine tasks on the server",
	"Access to remote servers",
	"Basics of SQL Create, Delete, Drop, Insert Into, Select, From, Where, Join",
	"Postgres database installation, configuration and use",
	"Non-relational database Redis installation, configuration and use",
	"Load testing in Jmeter",
	"Scrum development methodology",
	"Python. Learning the basics. Building a client-server application"
	]
}
Enter
Ctrl + D

 12. Отправить сразу 2 файла на внешний репозиторий.
git add preferences.json skills.json
git commit -m "add 2 files"
git push

 13. На веб интерфейсе создать файл bug_report.json.
Войти в репозиторий JSON. Нажать кнопку Add file.
Выбрать Create new file. В поле Name your file ввести bug_report.json

 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Нажать кнопку Commit new file

 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
Открыть файл bug_report.json Выбрать редактирование. Ввести текст
{
	"Bug_id":"5",
	"Title":"Top and bottom white dash line not visible for size W:242 H:546",
	"Severity":"Major",
	"Priority":"high",
	"Environment":[
			"Samsung Galaxy s10e, Android 12",
			"Samsung Galaxy М52, Android 11 ONE UI",
			"Samsung Galaxy S8, Android 9.0",
			"Samsung Galaxy Note 8, Android 9.0",
			"Samsung Galaxy A20, Android 11",
			"Samsung Galaxy A32, Android 11",
			"Samsung Galaxy A7, Android 10"
 			]
  	"Precondition":"Widget on Home screen 4x5",
	"STR":[ 
		"1. Open app",
		"2. Tap the "Add Widget" button",
		"3. Tap on the widget, start resizing"
		]
	"AR":"When resizing the widget W:242 H:546 the white dash lines above and below are not displayed"
	"ER":"When the widget is resized, the white dash lines along the outline are displayed"
	"Attachments":"https://disk.yandex.ru/i/J8npWOfTCPP6WA"
}

 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Нажать параметр Commit changes

 17. Синхронизировать внешний и локальный репозиторий JSON
git pull
