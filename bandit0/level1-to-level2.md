# LEVEL1 TO LEVEL2

Target: The password for the next level is stored in a file called - located in the home directory.<br>

This is similar to the level0-to-level1 challenge but the only thing that has changed is that the file name is a dash (-)<br>

we cannot use the direct cat command: cat - because it cannot open the file.<br>

Instead what we will be using is the cat < command to open the dash(-) filename.<br>

cat < - <br>

the password I found on my run is "263JGJPfgU6LtdEvgfWU1XP5yac29mFx"<br>

After that log in to the bandit2 account<br>

exit or logout<br>

ssh bandit2@bandit.labs.overthewire.org -p 2220.
