### Terminal. HW_2

**1.** Сделать папку `dir_1`
>$ mkdir dir_1

 **2.** Зайти в папку `dir_1`
>$ cd dir_1

 **3.** Создать папку `inner_dir_1`
>$ mkdir inner_dir_1

 **4.** Посмотреть, где ты находишься
>$ pwd

 **5.** Находясь в папке `dir_1`, создать пустой текстовый файл `tf_1.txt`
>$ touch tf_1.txt

 **6.** Находясь в папке `dir_1`, через команду **cat** создать текстовый файл `tf_2.txt` со следующими строками:
- the first 1
- the second 2
- the third 3
>$ cat > tf_2.txt  
the first 1  *`(Enter)`*  
the second 2 *`(Enter)`*  
the third 3 *`(Enter)`*
*`(Ctrl+C)`*

 **7.** Зайти в папку `inner_dir_1`
>$ cd inner_dir_1

 **8.** Через **cat** сделать текстовый файл `tf_3.txt`  c любыми строками
>$ cat > tf_3.txt  
line 1 *`(Enter)`*  
line 2 *`(Enter)`*  
line 3 *`(Enter)`*  
line 4 *`(Enter)`*  
line 5 *`(Enter)`*
*`(Ctrl+C)`*

 **9.** Через **cat** добавить в текстовый файл `tf_3.txt` строку “*the second 2*”
>$ cat >> tf_3.txt  
the second 2 *`(Enter)`*
*`(Ctrl+C)`*

 **10.** Через **cat** добавить в текстовый файл `tf_3.txt` строку “*the sec 2*”
>$ cat >> tf_3.txt  
the sec 2 *`(Enter)`*
*`(Ctrl+C)`*

 **11.** Через **cat** добавить в текстовый файл `tf_2.txt` строку “*the sec 3*”
>$ cat >> ../tf_2.txt  
the sec 3 *`(Enter)`*
*`(Ctrl+C)`*

 **12.** Через **cat** добавить в текстовый файл `tf_3.txt` строку “*the SeCoNd 2*”
>$ cat >> tf_3.txt  
the SeCoNd 2 *`(Enter)`*
*`(Ctrl+C)`*

 **13.** Через **cat** добавить в текстовый файл `tf_2.txt` строку “*the seConD 2*”
>$ cat >> ../tf_2.txt  
the seConD 2 *`(Enter)`*
*`(Ctrl+C)`*

 **14.** Сделать текстовый файл `tf_4.txt`, в котором будет 15 строк.
>$ cat > tf_4.txt  
line 1 *`(Enter)`*  
line 2 *`(Enter)`*  
line 3 *`(Enter)`*  
line 4 *`(Enter)`*  
line 5 *`(Enter)`*  
line 6 *`(Enter)`*  
line 7 *`(Enter)`*  
line 8 *`(Enter)`*  
line 9 *`(Enter)`*  
line 10 *`(Enter)`*  
line 11 *`(Enter)`*  
line 12 *`(Enter)`*  
line 13 *`(Enter)`*  
line 14 *`(Enter)`*  
line 15 *`(Enter)`*
*`(Ctrl+C)`*

 **15.** Сделать текстовый файл `tF_5.txt`, в котором будет 13 строк.
>$ cat > tF_5.txt  
string 1 *`(Enter)`*  
string 2 *`(Enter)`*  
string 3 *`(Enter)`*  
string 4 *`(Enter)`*  
string 5 *`(Enter)`*  
string 6 *`(Enter)`*  
string 7 *`(Enter)`*  
string 8 *`(Enter)`*  
string 9 *`(Enter)`*  
string 10 *`(Enter)`*  
string 11 *`(Enter)`*  
string 12 *`(Enter)`*  
string 13 *`(Enter)`*
*`(Ctrl+C)`*

 **16.** Вывести список всех файлов в папке.
>$ ls -la

 **17.** Выйти из папки `inner_dir_1`
>$ cd ..

 **18.** Вывести содержимое файла `tf_3.txt` в терминал.
>$ cat inner_dir_1/tf_3.txt

 **19.** Найти путь к файлу `tf_4.txt`
>$ find . -name tf_4.txt

*или*

>$ find ~+ -name tf_4.txt

 **20.** Очистить файл `tf_4.txt` от содержимого без удаления самого файла.
>$ > inner_dir_1/tf_4.txt

 **21.** Найти путь к файлам, у которых есть  “*tf*” в названии.
>$ find . -name '\*tf\*'

 **22.** Найти путь к файлам, у которых есть  “*tf*” в названии и буквы в любом регистре.
>$ find . -iname '\*tf\*'

 **23.** Найти строки в файлах, где есть комбинация букв “*sec*” в текущей папке
>$ grep sec \*.\*

 **24.** Найти строки в файлах, где есть комбинация букв “*sec*” в любом регистре в текущей папке
>$ grep -i sec \*.\*

 **25.** Найти строки в файлах, где есть только комбинация букв “*sec*” в текущей папке
>$ grep -w sec \*.\*

 **26.** Найти строки в файлах, где есть только комбинация букв “*sec*” в любом регистре в текущей папке
>$ grep -w -i sec \*.\*

 **27.** Найти строки в файлах, где есть комбинация букв “*second*” в текущей папке
>$ grep second \*.\*

 **28.** Найти строки в файлах, где есть комбинация букв “*second*” в любом регистре в текущей папке
>$ grep -i second \*.\*

 **29.** Найти строки в файлах, где есть комбинация букв “*second*” во всех папках ниже уровнем
>$ grep second \*/\*.\*

 **30.** Найти только путь и название файла, в строках которых есть комбинация букв “*second*” в текущей папке
>$ grep -l second \*.\*

 **31.** Найти все строки во всех файлах, где нет комбинации “*second*”
>$ grep -rv second

 **32.** Найти только название и путь к файлам, где нет комбинации “*second*”
>$ grep -lrv second

 **33.** Вывести в терминал 4 последние строки любого текстового файла.
>$ tail -n 4 inner_dir_1/tF_5.txt

 **34.** Вывести в терминал 4 первые строки любого текстового файла.
>$ head -n 4 inner_dir_1/tF_5.txt

 **35.** Команда в одну строку. Создать папку и создать текстовый файл с содержимым.
>$ mkdir inner_dir_2 | echo "some text" > tf_6.txt

 **36.** Команда в одну строку. Переместить в любую одну папку текстовые файлы, у которых в содержимом есть слово “*sec*”
>\$ mv -v \$(grep -wl "sec" \$(find . -iname "*.txt")) ./inner_dir_2

*либо*

>$ find . -iname "*.txt" | xargs grep -wl "sec" | xargs mv -t "./inner_dir_2"

*либо*

>$ find . -iname "*.txt" | xargs grep -wl "sec" | xargs -I @ mv @ "./inner_dir_2"

*либо*

>$ (find . -iname "*.txt" | xargs grep -wl "sec"; echo "./inner_dir_2" ) | xargs mv

*либо*

>$ find . -iname "*.txt" -exec grep -wl "sec" {} + | xargs mv -t ./inner_dir_2

 **37.** Команда в одну строку. Скопировать в любую одну папку текстовые файлы, у которых в содержимом есть слово “*sec*”.
>\$ cp -v \$(grep -wl "sec" \$(find . -iname "*.txt")) .

*либо*

>$ find . -iname "*.txt" | xargs grep -wl "sec" | xargs cp -t .

*либо*

>$ find . -iname "*.txt" | xargs grep -wl "sec" | xargs -I @ cp @ .

*либо*

>$ (find . -iname "*.txt" | xargs grep -wl "sec"; echo . ) | xargs cp

*либо*

>$ find . -iname "*.txt" -exec grep -wl "sec" {} + | xargs -I 123 cp 123 .

 **38.** Команда в одну строку. Найти все строки c “*sec*” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.
>\$ grep -h "sec" \$(find . -iname "*.txt") > tf_7.txt

*либо*

>$ find . -iname "*.txt" -exec grep -h --exclude=tf_7.txt "sec" {} + > tf_7.txt

*либо*

>$ find . -iname "*.txt" | xargs grep -h --exclude=tf_7.txt "sec" > tf_7.txt

*либо*

>$ find . -iname "*.txt" | xargs grep -h --exclude=tf_7.txt "sec" | cat > tf_7.txt

 **39.** Команда в одну строку. Удалить текстовые файлы, у которых в содержимом есть слово “*sec*”.
>\$ rm \$(grep -l "sec" \$(find . -iname "*.txt"))

*либо*

>$ find . -iname "*.txt" | xargs grep -wl "sec" | xargs rm

 **40.** Просто вывести в терминал строку “*Good job!!*”.
>$ echo 'Good job!!'
