# <a name="linux-command-line"></a>Linux Command Line

## Table of Contents
---
* [Overview](#a-nameoverviewaoverview)
* [File System](#a-namefile-systemafile-system)
* [Files and Directories](#a-namefile-and-directoriesafiles-and-directories)
* 

## <a name="overview"></a>Overview 
---
The Linux command line is a text interface to your computer. Often referred to as the shell, terminal, console, prompt or various other names, it can give the appearance of being complex and confusing to use. Yet the ability to copy and paste commands from a website, combined with the power and flexibility the command line offers, means that using it may be essential when trying to follow instructions online.

For more related resources visit [The Linux command line for beginners.](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)

## <a name="file-system"></a>File System
---
In Linux, directory structure starts with `/` symbol, which is referred as the `root` directory

* `man hier` gives description of the filesystem hierarchy. A few examples:
    * `/` This is the root directory. This is where the whole tree starts.

    * `/bin` This directory contains executable programs which are needed in single user mode and to bring the system up or repair it.

    * `/home` On machines with home directories for users, these are usually beneath this directory, directly or not. The structure of this directory depends on local administration decisions.

    * `/tmp` This directory contains temporary files which may be deleted with no notice, such as by a regular job or at system boot up.

    * `/usr` This directory is usually mounted from a separate partition. It should hold only sharable, read-only data, so that it can be mounted by various machines running Linux.

    * `/usr/bin` This is the primary directory for executable programs. Most programs executed by normal users which are not needed for booting or for repairing the system and which are not installed locally should be placed in this directory.

    * `/usr/share` This directory contains subdirectories with specific application data, that can be shared among different architectures of the same OS. Often one finds stuff here that used to live in /usr/doc or /usr/lib or /usr/man.

* For the Detail information of filesystem hierarchy type `man hier` in terminal.

##  <a name="file-and-directories"></a>Files and Directories
---
## pwd

>print name of current/working directory

* Apart from knowing your current working directory, often used to copy the absolute path to be pasted elsewhere, like in a script
* some Terminal emulators display the current directory path as window/tab title

```bash
$ pwd
/home/learnbyexample
```
* Full documentation at: <https://www.gnu.org/software/coreutils/pwd>

## <a name="cd"></a>cd

>Change the shell working directory

* Like `pwd`, the `cd` command is a shell builtin
```bash
$ pwd
/home/learnbyexample

$ cd /etc
$ pwd
/etc
```

**Further Reading**
* Use `help cd` for documentation
* [cd Q&A on unix stackexchange](https://unix.stackexchange.com/questions/tagged/cd-command?sort=votes&pageSize=15)
* [cd Q&A on stackoverflow](https://stackoverflow.com/questions/tagged/cd?sort=votes&pageSize=15)
## <a name="clear"></a>clear

>clear the terminal screen

You can also use `Ctrl+l` short-cut to clear the Terminal screen (in addition, this retains any typed text)

<br>

## <a name="ls"></a>ls

>list directory contents

* by default, `ls` output is sorted alphabetically

## <a name="mkdir"></a>mkdir

>make directories

* Linux filenames can use any character other than `/` and the ASCII NUL character
* Quote the arguments if name contains characters like space, `*`, etc to prevent shell interpretation
  
```bash

$ mkdir reports
$ ls
reports
```
#### For more related resources visit [Linux Directory Management](https://www.cyberciti.biz/tips/understanding-unixlinux-filesystem-directories.html)
<br>

## Working with Files and Folders
---
