### Welcome to level 0.

Here we need to log-in with a SSH terminal. Check out the full text over at http://overthewire.org/wargames/bandit/bandit0.html.

If you are using any Unix derivative (linux or MacOS) open a terminal and you can start a SSH connection. If you are on windows, you'll need to use a third party app, I recommend Putty or Multi-Putty based. Once you've got either one install you'll interactwith the GUI to log in.

On Terminal we use the command:
    `ssh Bandit.Labs.OverTheWire.org -p 2220 -l Bandit0`
    
If you don't know what SSH is, I suggest reading about it. SSH is best known for login into remote systems over an unsecure network. Here we are logging into OverTheWire's Wargaming server.

The flag `-p 2220` specifies that we want to connect over port 2220

The flag `-l Bandit0` specifies which user we are logging in as. 

If you are using Putty this should all be in the GUI interface.

Next our task is to read a file that contains the passcode to Bandit1. The file is stored as readme. The most straightforward way to do this is to use `cat` (the linux command for concatenate) which will print the files contents to the screen.

In terminal:
    `$ cat readme`
    
And we get the password for Level 1. 
> boJ9jbbUNNfktd78OOpsqOltutMc3MY1
 
