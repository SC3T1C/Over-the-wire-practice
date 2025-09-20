# LEVEL 5 TO LEVEL 6

Target: The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable<br>
1033 bytes in size<br>
not executable<br>

This case is similar to level 5 having a lot of files but this time, it has a lot of folders containing a lot files inside.<br>

If we check all the folders and all the files it will take a long time.<br>

So instead we will be using the find command to find the file with these components as given:

human-readable<br>
1033 bytes in size<br>
not executable<br>

Command: find . -type f -size 1033c ! -executable<br>

Explanation: 

find . -> find in the current directory or dot (.)<br>
-type f -> find the type f or find the file types<br>
-size 1033c -> find the files with 1033c or bytes (c)<br>
! -executable -> find the files that are not (!) executable<br>

In my case after running that command I found the file that fits the conditions: "./maybehere07/.file2"<br>

In order to check if that's human-readable then we will use the file command:

file ./maybehere07/.file2 which presented me with -> ASCII text, with very long lines (100), which means it is the human-readable file.

On my run after using the cat command, the password is "HWasnPhtq9AVKe0dmk45nxy20cvUa6EG"

then exit / logout and login to bandit6 with the ssh command.
