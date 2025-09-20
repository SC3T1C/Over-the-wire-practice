# LEVEL 3 TO LEVEL 4

Target: The password for the next level is stored in a hidden file in the inhere directory.<br>

The moment we log in to the bandit3 account/remote server, we are in the Home directory.<br>

The goal is to find a hidden file in the "inhere" directory.<br>

So the first thing to do is go inside the inhere directory with the cd command.<br>

cd inhere<br>

After we are inside the inhere directory, we cannot see the hidden file even if we use the ls or list command since this is a hidden command.<br>

What we need to do is to list all the files so we use the command:<br>

ls -a<br>

After that we can see the file named "...Hiding-From-You". If there are dots in the filename then we will also include that in the command.<br>

cat < ...Hiding-From-You<br>

The password I found on my run is "2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ"<br>

Then logout and exit and login to bandit4 with the ssh command.
