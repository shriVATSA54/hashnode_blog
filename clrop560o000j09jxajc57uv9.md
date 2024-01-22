---
title: "About Bash: You need To know!!!"
seoTitle: "Why Bash? and some basic commands."
seoDescription: "Discover the power of Bash shell! Uncover why Bash is essential and learn basic commands for streamlined efficiency. Elevate your command-line skills today"
datePublished: Mon Jan 22 2024 08:59:48 GMT+0000 (Coordinated Universal Time)
cuid: clrop560o000j09jxajc57uv9
slug: about-bash-you-need-to-know
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/4Mw7nkQDByk/upload/c968b8327e93be4f834136b86f89316a.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1705913053725/db930a7a-820f-4274-9ab0-158142fdb092.jpeg
tags: bash, linux-for-beginners, linux-commands

---

## Bash:

Bash is a comand(only commands) line interpreter(line by line execution) language that let's interact with Operating system.

It allows you to make directory,edit files ,copy many more.

Bash is commonly associated with Linux systems. Bash (Bourne Again SHell) is the default shell for many Linux distributions. Bash is not limited to only linux, it is also available for various unix-like sytems including MacOs, BSD etc. In Windows through a software called WSL(Windows Subsystem for Linux) can be accessed.

---

## Why Bash or any other command line Interface?

* ### Efficiency and Speed:
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705904815427/e74b065d-a8f8-47db-a98f-6cfb4311e7c2.webp align="center")

Working with CLI is faster and more efficient as compared to GUI(Graphical user interface). Within a few strokes/commands we can navigate, create, edit files or folders very quickly.

* ### Scripting and Automation:
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705905250014/b366d016-fa69-483c-9dd8-f103f5417dfa.webp align="center")

One of my favourite usecase is that through writing SCRIPT we can automate various repetative tasks and complex various workflows. By creating a script file wwe can use it multiple times by just one Command.

* ### **Resource Efficiency:**
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705905368806/15001d41-53aa-4b62-bb9e-7322cd06bb85.webp align="center")

CLI tools generally use fewer system resources than their GUI counterparts. This can be important in resource-constrained environments or when working on servers.

* ### **Scriptable Operations:**
    

CLI tools are inherently scriptable, allowing us to write many commands at one single file and execute all at one go.

* ### Portability:
    

Scripts written in Bash can be used across all other various unix-systems, allowing to create consistent solution across many Platforms.

* ### **Text-Based Output:**
    

CLI tools often provide text-based output, making it easier to parse, manipulate, and integrate with other tools. This is beneficial for tasks such as data processing and system monitoring.

---

## Some basic bash commands:

1. ls command: The `ls` (list) command is used to list directories or files.
    

* We can also use `ls -a` to view hidden files as well.
    
* `ls .extension` *to get all files, folders with that extension ex:* `ls *.txt`
    
* `ls startingletter*` gives all files, folders starrting with name specified. ex: ls new\*;
    
    ```bash
    ls 
    ls -a
    ls *.json
    ls name*
    ```
    

1. cd command: This allowsto change directory i.e., moving from one directory to another
    

* `cd foldername` enters to specified folder name.
    
* additionally we can also move inside nested folder in single command `cd foldername/foldername2`
    
* to move back one folder ie., to parent directory `cd ..`
    
    ```bash
    cd foldername/filename
    cd ..
    ```
    

1. pwd: This command gives us information about current working directory.
    

```bash
pwd
```

1. m command: mv stands to move, it litreallt is used to move a file/folder inside another folder. `mv project.txt NewFoldername`
    

`mv oldfile newFileName` to renamea file or folder

```bash
mv new.txt directoryTobeMoved
mv new.txt new2
```

1. rm command: used to delete file/folder
    

`rm specificDirectory` this deletes specific folfder

`rm -i` remove all files in directory

```bash
rm -i
```

1. cp : similar to mv command here a copy is created.
    

`cp oldFilename nrwFine`

```bash
cp new.txt Project
```

1. mdir command: This is useful when it comes to creating new directories in the file system.
    

* `mkdir newFolderName` creates new folder
    
* we can also create nested folders too `mkdir project/users/customer`
    

```bash
mkdir Project
```

1. touch command: this command is used to create a new empty file.
    

`touch newProject.txt` creates new file named newProject

```bash
touch Project.txt
```

1. Cat command: `cat` is a very commonly used command that allows users to read concatenate or write file contents to the standard output.
    

```bash
cat file.txt
```

1. grep command: grep is used to find a word/string in set of files.
    

`grep "string" filenName`

* grep -c "string" filename : gives number of line where "string" is present inside file
    
* grep -h "string" filename : gives no of occurance inside file
    
* grep -hir "string" : word inside entire directory
    
* grep -hin "string": line no's inside directory where string occurs
    

```bash
grep "price" users.txt 
```

1. vim command: This command is bit difficult to use. It is used to edit an existing file. Here are sequence of steps to follow.
    

* `vim filename.txt` to enter inside a file
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705912129621/f021dc13-2d09-4fab-8d8e-de6d0736aa19.png align="center")
    
* the interface now looks smntg like this
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705912166832/ba889872-2ca5-4608-9b6c-44a330ad277e.png align="center")
    
* ⚠️then no key works until we press `i` here i represnts: <mark>insert mode</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705912187319/54362dcc-308a-436d-8d41-c0a85ffb030d.png align="center")
    
* now can we make some changes inside file: here I have written "The new File This is vim command in use"
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705912226751/c9776a74-f908-4653-836d-9322e4395b46.png align="center")

* to exit we need to press: `esc : q !`
    
* to save and exit we need to enter `esc : w q !`
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705912465060/4d2aa573-73da-455c-89bc-ee1ffa63d84e.png align="center")

---

### Some popular website to practise:

* replit is online browser that allows to code and compile [link](https://replit.com/languages/bash)
    
* also [webminal](https://www.webminal.org/) provides environment and free tutorial to get good at bash
    

---

### Thanks for reading.!!!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705912972038/c03dc04a-47ec-4aee-9649-2b838c249d23.webp align="center")

***<mark>What is your favourite command??</mark>***

Connect me on [X](https://twitter.com/SHRIvatsa_desai)