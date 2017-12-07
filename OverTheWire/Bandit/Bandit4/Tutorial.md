Exact Instructions and helpful reading material over at http://overthewire.org/wargames/bandit/bandit5.html.

>Previous Tutorials Password: pIwrPrtPN36QITSp3EQaw936yaFoFgAB

It's time to start searching, for the next few levels we'll be looking at how to find files from the command line that contain certain elements. One obvious solution is to start opening the files one at a time and looking at their contents, but we want a more elegant solution.

Introducing `file`.

When we run `file /somewhere/something` it will tell us some of the attributes about that file, largely what that file contains. 

Let's begin our challenge. We need to find the only file that is human readable. Lets see what our options are.

`ls -a`
>inhere
`ls -a`
>./-file00

>./-file01

>./-file02

>./-file03

>./-file04

And so on..

What we can do is run `file ./-*`. The `*` is called the wildcard character, it will let any character or string of characters complete the command, showing us the results of **all** the files that start with `./-`.

`file ./-*`
>./-file00: data

>./-file01: data

....
>./-file07: ASCII text

`cat ./-file07`
>koReBOKuIDDepwhWk7jZC0RTdopnAYKh
