**Lab Report 1, Afraz Hameed**

cd with no arguments:

> user@sahara ~[lecture1]$ cd
> [user@sahara ~]$ 

cd with path to directory:

> user@sahara ~]$ cd lecture1
> [user@sahara ~lecture1]$

cd with path to file:

> cd lecture1/messages/ja.txt
> bash: cd: lecture1/messages/ja.txt: Not a Directory

cd is to move to a different directory, so when cd is called with no argument, nothing happens, and when you call it with a file as an argument, then it displays an error that it is not a directory, since cd only works with directories. However, with a directory used as an argument the next line will change and append the directory to the end of user@sahara, showing the directory changed.
---

ls with no arguments:

> [user@sahara~]$ ls 
> lecture1 test

ls with path to directory:

> [user@sahara~]$ ls lecture1
> Hello.class Hello.java messages README

ls with path to file:
> [user@sahara~]$ ls lecture1/README
> lecture1/readme

ls means to list out all the ocntents of a folder/directory. When using ls with no arguments, it simply lists out the current working directory and the content in it, files, folders, etc. With a directory as an argument, it shows all the files/directories inside that directory. When calling ls with a file, it just gives the same thing back out as output, with the file name, since ywhen listing a file there's nothing that that file has to list out as no other items belong to the file, so there is no extra output produced.
---

cat with no arguments:

> [user@sahara~]$ cat
> (Nothing happens)


cat with path to directory:
> [user@sahara~]$ cat lecture1
> cat: lecture1: Is a directory


cat with path to file:
> [user@sahara~]$ cat lecture1 lecture1/README
> To use this program:
>
> javac Hello.java
> java Hello messages/en-us.txt

Cat is a command to conacatenate / print the contents of whatever files that are called. When using cat with no argument, there is no output produced since there is nothing to print. When using cat with a directory, a message pops up clarifying that the argument is a directory, showing clarification that you can't use cat and print out the folder since it contains other items that can be printed instead. Finally, using cat with actual files prints the actual contents of it, whether it's a txt or a class file, it prints out all the code/words that are included in the file's contents.
