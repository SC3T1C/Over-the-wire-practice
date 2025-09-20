# LEVEL 6 TO LEVEL 7 

Target: The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

This case is very similar to level6 with the conditions given that we need to follow.<br>

The only difference is that instead of a folder or a directory, we will be finding the password in the whole server.<br>

So for that we will use the find command with some conditions that fit the conditions that we are finding.<br>

command: 

find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null<br>

Explanation:

/ → start searching from the root directory<br>

-type f → only look for files<br>

-user bandit7 → must be owned by user bandit7<br>

-group bandit6 → must be owned by group bandit6<br>

-size 33c → must be exactly 33 bytes (c = bytes)<br>

2>/dev/null → hides all the “Permission denied” spam you’d otherwise see<br>

After running that command, I was presented with the directory that fits the condition givem: "/var/lib/dpkg/info/bandit7.password"<br>

In my run after reading the file with the cat command, I was presented with the password "morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj"

Then exit / logout and login to bandit7 using the ssh command.

