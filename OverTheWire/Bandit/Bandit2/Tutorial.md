Exact Instructions and helpful reading material over at http://overthewire.org/wargames/bandit/bandit2.html.

> Previous Tutorials Password: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

In this challenge we will continue where we left off last tutorial exploring the file system. Once logged in the instructions tell us that the password is in a file named **spaces in this filename**. 

If you read the tutorial for Bandit1, youd already know one answer to this is to treat the name as a sting using qoutation marks. Then when we ask the terminal to find the file, it will compare strings to filenames.

	`cat "spaces in this filename"`

Giving us:

> Bandit3's Password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
