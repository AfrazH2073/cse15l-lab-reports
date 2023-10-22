**Lab Report 1, Afraz Hameed**

**cd with no arguments:**
![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/242f6390-8388-49ac-a6aa-476f40954ccf)

The cd command asks for a parameter of a directory to change directories to. Since there was no directory given as a parameter, the output resulted in an error since there was no directory referenced to switch to, so the command didn't print anything else after.

**cd with path to directory:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/4c02e7c7-aa71-4441-b62b-132c68a78812)

The cd command was run to switch directories to /home/lecture1/messages, which worked, as shown by the second line resulting in [user@sahara ~]$ becoming [user@sahara ~/lecture1/messages]$. 
cd with path to file. There weren't any results that printed but we can see that the working directory now changed.

**cd with path to file:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/6ec1b6b9-72bb-4194-a7b1-68973208236e)


Running cd with a file gives us an error that the file is Not a directory, which makes sense, because cd requires the argument be a directory to switch to. However, when trying to cd with a file, the file destination gets regurgitated back out to us with no changes being made to our directory.

---

**ls with no arguments:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/7299990b-d424-4f1d-82a3-598ecf51d6ca)

ls with no arguments lists out all the directories and files present within the current working directory we are in. Therefore, when using ls we got to see all the directories/files present within our home directory, which included lecture1 and test. lecture1 is bolded since it is a directory, and test is not bolded because it's just a file, no errors occurred.

**ls with path to directory:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/44118a0b-9163-42b3-b903-cdc433e9cd2d)

When using ls with a path to directory, the program lists out all the directories/text in the directory that we called. We called ls with the path to /home/lecture1, so the program displayed all directories and files present within that directory, even if our working directory was the home directory, and no errors were thrown throughout this process.

**ls with path to file:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/5143cc5b-9212-45cb-aeba-9c72abeb9283)


Using ls and running it by calling it with a file results in an error being thrown. The error simply outputs the same path we inputted back towards us, showing that ls does not work with a file, the reason being that ls lists out the directories/files that are under a directory- so a file can't have those kinds of items under itself, since a file is the most specific path you can have, therefore there is nothing else to list. 

---

**cat with no arguments:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/9343fc0e-5725-4b8a-8732-37bbf3e6cb85)

Cat method is designated to print the contents of a file, and therefore since there is no file in the arguments, there is nothing to print, therefore it's an error- nothing is printed in return.

**cat with path to directory:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/62830907-9ff4-4e14-b9de-1d8cec2a4e85)

Using cat with a directory simply returns an error message clarifying that the path we inputted is a directory. This error is thrown since cat is used to print contents of a file, and therefore if you have a directory, you can't print out the contents of a directory with cat since it doesn't have text/code in it- it has files and directories in it. 

**cat with path to file:**

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/7826a169-78e6-40ce-b545-57f7ad01db22)

Using cat with a file prints out the text/content of the actual file, since the intended parameter for the cat command is a file. No errors were made, as the content was printed successfully.

---
