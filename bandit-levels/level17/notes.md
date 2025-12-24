## Goal
There are two files in the home directory:passwords.new and passwords.
old.The passwords for the nect level is in passwords.new and is the 
only line that has been changed between passwords.old and passwords.new
NOTE:if you have solved this level and see 'Byebye!'when trying to log
into bandit 18,this is related to the next level,bandit19.

## Solution
ls
diff passwords.new passwords.old

## Explanation
diff compares two files line by line.It ouputs only the differences
between them.Since the files are almost identical,the one changed line
is the password for the next level.The line starting with > shows the
line that exists only in the new file.

## Password
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

## Key Lesson
When comparing files,diff is the fastest way to spot changes.Its common-
-ly used to detect configuration changes,file updates.
