# LEVEL 4 TO LEVEL 5

Target: The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.<br>

This is similar to level 4 with the "inhere" directory and the ls files but the goal here is to find the only "human-readble" file in this directory.<br>

If we use ls or ls -a we are presented with a lot of files, and manually using the cat command on all these files will take a long time.<br>

So instead we are going to be using the file command, specifically the comand "find ./*". This command allows us to view all the files plus what they contain(data, ASCII text, etc.)<br>

After using the file ./* command we can see which file is the human-readable file or the file with the ASCII text data.<br>

On my run it is the -file07 and it contained the password "4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw"<br>

Then exit / logout and login to bandit5 with the ssh command.
