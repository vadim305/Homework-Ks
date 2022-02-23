1) Посмотреть где я ---pwd
2) Создать папку ---mkdir (example $ mkdir test)

3) Зайти в папку ---cd (example $ cd test)
4) Создать 3 папки ---(example $ mkdir test{1,2,3} )

5) Зайти в любою папку ---(example cd test1)
6) Создать 5 файлов (3 txt, 2 json) ---(example $ touch file_txt{1,2,3}.txt)
($ touch file_json{1..2}.json)

7) Создать 3 папки ---(example $ mkdir folder_{1..3})

8. Вывести список содержимого папки --- (example ls -la) или (ls)
9) + Открыть любой txt файл ---(example   $ vim file_txt1.txt)
10) + написать туда что-нибудь, любой текст. ---(работа в редакторе, потом esc :wq Enter) 
11) + сохранить и выйти. 

12) Выйти из папки на уровень выше ---(example $ cd ..)
13) переместить любые 2 файла, которые вы создали, в любую другую папку. ---(example $ mv *.json folder_1/)- переместил все файлы с расширением .json
(example $ mv file_txt1.txt file_txt2.txt folder_1/)- переместил в другую папку 2 файла 


14) скопировать любые 2 файла, которые вы создали, в любую другую папку. ---(example $ cp file_txt1.txt file_txt2.txt ~/test/test1/folder_2)-указал абсолютный адрес
при копировании файлов.

15) Найти файл по имени --- 
(example  ~/test/test1/folder_2
$ find file_txt1.txt
file_txt1.txt) 
или в данном случае поиск двух ранее копированных файлов 
(example ~/test/test1
$ find . -name file_txt2.txt
./folder_1/file_txt2.txt
./folder_2/file_txt2.txt )


16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. --- (example $ tail -f file_txt1.txt)
cat file_txt3.txt | grep tea ---  ищет слово сдержащиеся в файле или его часть.





17) вывести несколько первых строк из текстового файла --- (example $ head file_txt1.txt)

18) вывести несколько последних строк из текстового файла --- (example $ tail file_txt1.txt)

19) просмотреть содержимое длинного файла (команда less) изучите как она работает. --- ( example $ less file_txt1.txt) 
после просмотра файла нажать ESC попадем в терминал

20) вывести дату и время --- (example $ date
Thu Feb 10 21:22:09     2022)

=========

Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request ---( example $ curl http://162.55.220.72:5005/terminal-hw-request
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   237  100   237    0     0    400      0 --:--:-- --:--:-- --:--:--   400{"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}
(EXAMPLE)
$ curl "http://162.55.220.72:5005/get_method?name=(vadim)&age=(32)"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    19  100    19    0     0    211      0 --:--:-- --:--:-- --:--:--   213["(vadim)","(32)"]





2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 --- example
#!/bin/bash
cd test
mkdir test{8,9,10}
cd test9
touch touch file_json{1..5}.json
mkdir folder_{1..3}
ls -la
mv file_json1.json file_json2.json folder_2/

скрипт был написан в nano-редакторе 
далее ctrl+O для сохранения скрипта ( имя для сохранения :123 )
далее ctrl+X для выхода из редактора
исполнение скпипта в терминале: ./123





=====================
1) Посмотреть где я - pwd --- $ pwd
/c/Users/harbo

2) Создать папку - mkdir foldername
3) Зайти в папку - cd foldername
useless@advice MINGW64 ~


$ mkdir foldername-------------создал

useless@advice MINGW64 ~
$ cd foldername  -----------------вошел

useless@advice MINGW64 ~/foldername  



