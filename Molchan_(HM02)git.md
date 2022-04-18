Как отправить ДЗ на проверку.
 1. Создайте текстоовый файл как в первом ДЗ по Terminal.
 2. Сценарий перенесите в этот файл.
 3. На против каждого действия - напишите команду в GitBash

Файл со сценарием и ссылку на свой гит хаб отправляйте менторам на проверку.

JSON
 4. Создать внешний репозиторий c названием JSON. --- создание репозитория на github.com c именем JSON 
Перейдите на https://github.com и войдите в свой аккаунт. 
Нажмите кнопку New repository (JSON ). На открывшейся странице введите имя репозитория (Repository name) и нажмите кнопку Create repository.
 Данная команда добавит удаленный репозиторий с именем JSON  , который указывает на ваш Github-репозиторий.
 5. Клонировать репозиторий JSON на локальный компьютер. --- $ git clone https://github.com/vadim305/JSON.git
пояснение:
клонирование репозитория на локальный компьютер происходит в заранее выбранную папку 
useless@advice MINGW64 /d/testing/home
$ git clone https://github.com/vadim305/JSON
Cloning into 'JSON'...
далее 
useless@advice MINGW64 /d/testing/home
$ cd json
далее
useless@advice MINGW64 /d/testing/home/json (main)
$


 6. Внутри локального JSON создать файл “new.json”. --- $ touch new.json

 7. Добавить файл под гит. --- $ git add new.json

 8. Закоммитить файл. --- $ git commit -m "born new.json"


 9. Отправить файл на внешний GitHub репозиторий. --- $ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 270 bytes | 270.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/vadim305/JSON
   54411a2..901d02e  main -> main

 10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних  животных, будущая желаемая зарплата). Всё написать в формате JSON. ---
$ cat >> new.json
new
{"name": "Molchan_Vadim_Igorevich",
"age": 32,
"home_animals": null,
"future_salary": 350
}



 11. Отправить изменения на внешний репозиторий. --- 
$ git add new.json  --- написал изменения (текст) в new.json 
$ git commit -m "I writed down it in new.json" 
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 401 bytes | 401.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/vadim305/JSON
   901d02e..7cb449b  main -> main

ПРИМЕЧАНИЕ также использовал команду git status для отображения текущего состояния файла 

 12. Создать файл preferences.json --- в терминале GitBash в /d/testing/home/JSON (main) создается файл  preferences.json 
$ touch preferences.json

 13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON. ---
с помощью редактора nano добавляю текст с содержимым  (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) 
сохранение в nano: ctrl + x + y
$ cat  preferences.json --- проверка содержимого файла
редактирую с помощью редактора nano 
команда gitbash 
nano preferences.json
preferrences
{"favorite_movie": "Taxi",
"favorite_show": "Supernatural",
"food": ["pizza","burger","bread"],
"season": "spring",
"visit": "Poland"
}
сохраняю в nano

 14. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON --- 
$ touch sklls.json
далее через редактор nano редактирую файл под содержимое требований задания
sklls
{"skils": ["git","postman","jmeter","other"]
}

сохраняю в nano
проверяю git status 
preferences.json
sklls.json
эти два файла в терминале подсвечены красным


 15. Отправить сразу 2 файла на внешний репозиторий. --- 
$  git add . | git commit -m 



 16. На веб интерфейсе создать файл bug_report.json. --- работа в GitHub в репозитории JSON создаю bug_report.json
Входим на свой репозиторий (https://github.com/vadim305 ) — создаю 
 bug_report.json в репозитории JSON
нажимаю добавить файл
нажимаю создать новый файл 
предлагается назвать файл в репозитории JSON 
ввожу имя bug_report.json
внизу страницы зеленая кнопка
зафиксировать новый файл нажимаю
файл создан.
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе. --- сохранил в github 
входим в репозиторий JSON
выбираем нужный файл  bug_report.json
нажимаем на имя файла bug_report.json 
открывается 
https://github.com/vadim305/JSON/blob/main/bug_report.json нажимаем кнопку изменить этот файл (в виде "карандаш")
правим текст файла
 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
{
"tester":"Molchan",
 "data":"18_April_2022",
   "title":"JSON_example_bug",
   "summary":"text support pages has grammar mistakes",
   "platform":"windows",
   "priority":"low",
   "severite":"low",
   "status":"new",
   "author":"Molchan"
}

 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе. --- сохранил в github 
после правки текста нажимаем зеленую кнопку зафиксировать изменения 
 20. Синхронизировать внешний и локальный репозиторий JSON --- в терминале использовать команду git pull - скачачивает изменения с сервера  github  на компьютер 


XML
 21. Создать внешний репозиторий c названием XML. --- в GitHub через интерфейс создается репозиторий
Перейдите на https://github.com и войдите в свой аккаунт. 
Нажмите кнопку New repository   (XML). На открывшейся странице введите имя репозитория (Repository name) и нажмите кнопку Create repository.
 Данная команда добавит удаленный репозиторий с именем XML  , который указывает на ваш Github-репозиторий.

 22. Клонировать репозиторий XML на локальный компьютер. --- в терминале useless@advice MINGW64 /d/testing/home/JSON (main)
$ cd -
/d/testing/home
с помощью cd -     возвращаюсь в папку home 
 синхронизирую новый XML репозиторий посредством $ git clone https://github.com/vadim305/XML
 23. Внутри локального XML создать файл “new.xml”. --- $ touch new.xml 
git status файл new.xml подсвечен красным
 24. Добавить файл под гит. --- $ git status
$ git add .
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.xml  --- подсвечен зеленым 

 25. Закоммитить файл. --- $ git commit -m "born new.xml"

 26. Отправить файл на внешний GitHub репозиторий. --- $ git push
в репозитории XML на GitHub при обновлении страницы появляется new.xml
27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML. --- $ nano new.xml
в редакторе делаю изменения сохраняю.
<?xml version="1.0" encoding="UTF-8" ?>
<root>
    <name>Molchan_Vadim_Igorevich</name>
    <age>32</age>
    <home_animals />
    <future_salary>350</future_salary>
</root>
 28. Отправить изменения на внешний репозиторий. ---  git status new.xml красный 
$ git add new.xml 
$ git commit -m "I maked commit in file new.xml"
$ git status new.xml 
$ git push

 29. Создать файл preferences.xml --- 
 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML. ---

создал с помощью команды touch  preferences.xml  в редакторе nano сделал запись и сохранил. git status подсвечивает файл preferences.xml красным
<?xml version="1.0" encoding="UTF-8" ?>
<root>
    <favorite_movie>Taxi</favorite_movie>
    <favorite_show>Supernatural</favorite_show>
    <food>pizza</food>
    <food>burger</food>
    <food>bread</food>
    <season>spring</season>
    <visit>Poland</visit>
</root>
 31. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML --- touch sklls.xml после в редакторе nano добавляю текст сохраняю ctrl+ x + yes
<?xml version="1.0" encoding="UTF-8" ?>
<root>
    <skils>git</skils>
    <skils>postman</skils>
    <skils>jmeter</skils>
    <skils>other</skils>
</root>
 32. Сделать коммит в одну строку. --- $  git add . | git commit -m 
 33. Отправить сразу 2 файла на внешний репозиторий. --- $ git push 
после 
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

 34. На веб интерфейсе создать файл bug_report.xml. --- переход в GitHub в репозитории XML создаю файл bug_report.xml (GitHub)
Входим на свой репозиторий (https://github.com/vadim305 ) — создаю 
 bug_report.xml в репозитории XML
нажимаю добавить файл
нажимаю создать новый файл 
предлагается назвать файл в репозитории XML
ввожу имя bug_report.xml
внизу страницы зеленая кнопка
зафиксировать новый файл нажимаю
файл создан.
 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе. --- сохранение (GitHub) входим в репозиторий XML
выбираем нужный файл  bug_report.xml
нажимаем на имя файла bug_report.xml
открывается 
https://github.com/vadim305/JSON/blob/main/bug_report.xml нажимаем кнопку изменить этот файл (в виде "карандаш")
правим текст файла

 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML. --- в репозитории XML, в файле bug_report.xml записал 

<root>
   <author>Molchan</author>
   <data>18_April_2022</data>
   <platform>windows</platform>
   <priority>low</priority>
   <severite>low</severite>
   <status>new</status>
   <summary>text support pages has grammar mistakes</summary>
   <tester>Molchan</tester>
   <title>XML_example_bug</title>
</root>
 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе. ---
 после правки текста нажимаем зеленую кнопку зафиксировать изменения 
сохранил, обновил страницу, файл есть в репозитории XML  (Git Hub)

 38. Синхронизировать внешний и локальный репозиторий XML  --- работа в терминале GitBash на локальном компьютере
$ git pull





TXT
 1. Создать внешний репозиторий c названием TXT. --- создание в GitHub репозитория TXT 
 Перейдите на https://github.com и войдите в свой аккаунт. 
Нажмите кнопку New repository   (TXT ). На открывшейся странице введите имя репозитория (Repository name) и нажмите кнопку Create repository.
 Данная команда добавит удаленный репозиторий с именем TXT   , который указывает на ваш Github-репозиторий.
 2. Клонировать репозиторий TXT на локальный компьютер. --- gitbash ---  
$ git clone https://github.com/vadim305/TXT
Cloning into 'TXT'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.



 3. Внутри локального TXT создать файл “new.txt”. --- внутри TXT(main) --- создание файла touch new.txt

 4. Добавить файл под гит. --- $ git add new.txt

 5. Закоммитить файл. --- $ git commit -m "born new.txt"

 6. Отправить файл на внешний GitHub репозиторий. ---  $ git push



 7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.
 --- $ nano new.txt
с помощью редактора вносятся изменения в файл 
  8. Отправить изменения на внешний репозиторий. --- 
$ git add .
$ git commit -m
$ git push


  9. Создать файл preferences.txt --- touch preferences.txt в gitbash в ветке TXT (main)


 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT ---. $ cat >> preferences.txt

 11. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT --- $ touch sklls.txt (создание файла) -$ cat >> sklls.txt (мой текст) сохранение изменений в файле ctrl +c

 
 12. Сделать коммит в одну строку. --- $ git add  preferences.txt sklls.txt
   git add . | git commit -m 


 13. Отправить сразу 2 файла на внешний репозиторий. --- git push
 14. На веб интерфейсе создать файл bug_report.txt.---  bug_report.txt. создание в Github
переход в своем аккаунте в репозиторий TXT 
нажимаю добавить файл
нажимаю создать новый файл 
предлагается назвать файл в репозитории TXT
ввожу имя bug_report.txt
внизу страницы зеленая кнопка
зафиксировать новый файл нажимаю
файл создан.
 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе. --- сохранение в Github
входим в репозиторий TXT
выбираем нужный файл  bug_report.txt
нажимаем на имя файла bug_report.txt
открывается 
https://github.com/vadim305/JSON/blob/main/bug_report.txt нажимаем кнопку изменить этот файл (в виде "карандаш")
правим текст файла
 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT. --- сделал запись в файл
 bug
Короткое описание (Summary)	Автор баг репорта (обычно это Тестировщик)
Проект (Project)	Автор баг репорта (обычно это Тестировщик)
Компонент приложения (Component)	Автор баг репорта (обычно это Тестировщик)
Номер версии (Version)	Автор баг репорта (обычно это Тестировщик)
Серьезность (Severity)	Автор баг репорта (обычно это Тестировщик), однако данный атрибут может быть изменен вышестоящим менеджером
Приоритет (Priority)	Менеджер проекта или менеджер ответственный за разработку компонента, на который написан баг репорт
Статус (Status)	Автор баг репорта (обычно это Тестировщик), но многие системы баг трекинга выставляют статус по умолчанию
Автор (Author)	Устанавливается по умолчанию, если нет, то указывается имя автора баг репорта
Назначен на (Assigned To)	Менеджер проекта или менеджер ответственный за разработку компонента, на который написан баг репорт
ОС / Сервис Пак и т.д. / Браузера + версия / ...	Автор баг репорта (обычно это Тестировщик)
Шаги воспроизведения (Steps to Reproduce)	Автор баг репорта (обычно это Тестировщик)
Фактический Результат (Result)	Автор баг репорта (обычно это Тестировщик)
Ожидаемый результат (Expected Result)	Автор баг репорта (обычно это Тестировщик)

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе. сохранил в Github
 после правки текста нажимаем зеленую кнопку зафиксировать изменения 
сохранил, обновил страницу, файл есть в репозитории  TXT (Git Hub)
 18. Синхронизировать внешний и локальный репозиторий TXT --- $ git pull
