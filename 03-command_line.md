# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 1. pwd - show current working directory path
> > 2. mkdir [directory] - create a new directory
> > 3. rm -r [directory] - deletes a directory and all of its contents
> > 4. touch [filename] - creates an empty file
> > 5. rm [filename] - removes the specified file
> > 6. mv [old filename] [new filename] - renames the old filename to the new filename
> > 7. ls -a - lists all files, including the hidden files
> > 8. cp [directory/filename] [destination directory] - copies a file to a directory
> > 9. grep -R [phrase] - search in all files in the current directory for the provided phrae
> > 10. less [filename] - displays the contents of a file and able to page through the file

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > `ls` - lists all files in the current working directory, except hidden files  
> > `ls -a` - list all files including hidden files  
> > `ls -l` - list all non-hidden files in a long format  
> > `ls -lh`  - list all non-hidden files in a long format and use unit suffixes: Byte, Kilobyte, Megabyte, Gigabyte, Terabyte, and Petabyte.
> > `ls -lah` - list all files in a long format and use unit suffixes: Byte, Kilobyte, Megabyte, Gigabyte, Terabyte, and Petabyte.
> > `ls -t` - list non-hidden files in sorted by modified time  
> > `ls -Glp` - list non-hidden files with color and add '/' if it is directory 

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 1. ls -m - displays the names as a comma-separated list
> > 2. ls -p - displays the directories with /
> > 3. ls -R - displays subdirectories as well
> > 4. ls -u - displays files by the file access time
> > 5. ls -d - displays only directories 

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 'xargs' reads STDIN stream of data and converts into space separated arugments to the commnand. For example, executing 'xargs -L 1 touch' will use STDIN and submit line by line as an argument for the touch command.
 

 

