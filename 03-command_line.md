# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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

> > pwd - show current working directory path
cd - create directory
rmdir - delete directory
touch - create a file
rm - delete file
mv - rename a file
defaults - listing hidden files
cp - copying files
ls - listing files in current directory
open . - open the directory
q - exit
clear - clear screen
ctrl + c - kill whatever you're running

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

> > ls - list files in working directory
ls -a - list all files, including hidden ones
ls -l - list all files in its long form
ls -lh - lists all files in its long form and its respective size
ls -lah - lists all files, including hidden ones, in its long form    and its respective size
ls -t - lists all files in the order in which they were last modified
ls - Glp - lists all files in its long form
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > -r: displays files in reverse order
-x: displays files as rows across the screen
-m: displays the names a comma separated list
-d: displays only directories
-C: displays files in a column format

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 'xargs' is used to build and execute command lines from standard input. It allows functions, that usually solely rely on arguments found after the command, to use the standard input or items from pipes as the input. Also sometimes, long lists of parameters can't be passed to a command, so xargs breaks the list of arguments into sublists small enough to be acceptable.Here's an example on how to use 'xargs': $ echo 1 2 3 4 | xargs echo. This prints (1 2 3 4) at once.
 

