Exact Instructions and helpful reading material over at http://overthewire.org/wargames/bandit/bandit2.html. 

> Previous Tutorials Password: boJ9jbbUNNfktd78OOpsqOltutMc3MY1

For this challenge and the next several we begin exploring the linux file system, how it's organized and good ways of how to use it. For this challenge the password is stored in a file named - in the home directory.

Before we begin let me introduce "ls" the linux command for listing whats in the current folder. Most often I will use "-a" flag to list all files and paths. I can also use the "-al" flag to include file permissions, access times and who wrote/read the file.

As in Bandit0 we can use "cat -" to read the file, except it wont work. Linux wont recognize "-" as a file because it is a special character. To get around this I've found a few different ways.

Option #1: Qoutes
    By putting anything in qoutes, terminal will read it as a string. Then by using 'cat "Something"' terminal will treat that
    something as string and see if there is a file with a matching string name.
    
    `~$ cat "-"`
    
Option #2: Understanding ./-
    In the Linux file structure . refers to the current directory and .. refers to the directory one level up (the direcotry that
    the current directory is in). By using ./something terminal will look in the current directory for something. We can also use
    ~ to reference root, or base level. In more advanced useage we can quickly reference other files by referring to them in the
    directory/subdirectory/file way.
    
    `~$ cat ./-`
    
Terminal should then spit out the password for Bandit2.
    CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
