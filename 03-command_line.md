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

> > * show current working directory path
  
  cd
  
* creating a directory
  
  mkdir
* deleting a directory
  
  rmdir
* creating a file using `touch` command
  
  touch filen.ext
* deleting a file
  
  rm filen.ext
* renaming a file
  
  mv (option) file1.ext file2.ext
* listing hidden files
  
  ls -ld .?* 
* copying a file from one directory to another
  
  cp filen.ext newdirectory/
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

Response:
`ls` : list all files and directories.

`ls -a`: lists all entries including those starting with periods (.), but excluding any . or .. entries.  

`ls -l`:  displays permissions, links, owner, group, size, time, name; 

`ls -lh`:  displays permissions, links, owner, group, size, time, name; also displays file sizes using more human-friendly units. 

`ls -lah`:  Lists all entries including those starting with periods (.);displays permissions, links, owner, group, size, time, name; also displays file sizes using more human-friendly units. 

`ls -t`: sorts entries by time. By default, this option sorts the output by the modification times of files. 

`ls -Glp`: displays permissions, links, owner, group, size, time, name; puts / after directory names; displays only the group ID numbers 

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > -a	Displays all files.

-d	Displays only directories.

-l	Displays the long format listing.

-t	Displays newest files first. (based on timestamp)

-R	Displays subdirectories as well.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs is a command on Unix and most Unix-like operating systems used to build and execute command lines from standard input. xargs breaks the list of arguments into sublists small enough to be acceptable.

Example:

find /path -type f -print | xargs rm

In the above example, the find utility feeds the input of xargs with a long list of file names. xargs then splits this list into sublists and calls rm once for every sublist.

 

