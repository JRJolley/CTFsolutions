Exact Instructions and helpful reading material over at http://overthewire.org/wargames/bandit/bandit4.html.

> Previous Tutorials Password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

Now that we've gotten comfortable opening files and interacting with different filenames this challenge asks us to navigate directories. Specifically to open a hidden file in the **inhere** directory.

Introducing `cd` which is short for change directory. By entering `cd destination` we will change our working directory to the destination directory. For this challenge we will use:

	cd inhere

You should notice that our console name has changed from `bandit3@bandit: ~$` to `bandit3@bandit: ~/inhere$` indicating that we are acting inside of the inhere directory.

In an earlier tutorial I introduced the `ls` command, which will list all of the objects in your working directory. If we run `ls` right now, the terminal will find nothing. But by adding the `-a` or display all flag we will see all objects including the links `.` and `..` for here and up a level, as well as any interesting files.
	
	ls -a

>.hidden

	cat .hidden

> pIwrPrtPN36QITSp3EQaw936yaFoFgAB
