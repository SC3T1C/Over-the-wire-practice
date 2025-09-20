# level0-to-level1

target: The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.<br>

commands used:<br>

Since our goal is to find and read the "readme" file then the first command would be "ls" or list files in the directory.<br>
Then access the readme file using "cat" command to read the file. command: cat readme<br>

After that the password can be found in the readme file. The example password or my run is "ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If" <br>

then exit or logout and login to bandit1 using that password.<br>

ssh bandit1@bandit.labs.overthewire.org -p 2220
