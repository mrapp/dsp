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

> > * show current working directory path: 'ls'
* creating a directory: `mkdir` directory 
* deleting a directory: `rm -r` directory
* creating a file using `touch` command: `touch` filename
* deleting a file: `rm` filename
* renaming a file: `mv` oldfilename newfilename
* listing hidden files: `ls -a`
* copying a file from one directory to another: `cp` oldfilename newfilename path
* move a file: `mv` filename path
* read file to standard output: `cat` filename
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

> > `ls`: list directory   
`ls -a`: list directory including hidden files  
`ls -l`: list directory long, includes lots of additional info  
`ls -lh`: list directory long with abbreviated file sizes  
`ls -lah`: lists directory long with abbreviated file sizes including hidden files  
`ls -t`: list directory sorted by date modified  
`ls -Glp`  : lists directory long with blue directories and a "/" at the end of directories

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > * `-R` displays subdirectories as well
* `-g` displays long excluding owner's name
* `-d` displays only directories
* `-m` displays files in comma seperated list
* `-q` displays non-printing charectors as "?"

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > It reads the standard in and applys it to a command as argument. For examaple, `ls *.md | xargs grep "Unix"` is equivelant to `grep "Unix" *.md`.

 

