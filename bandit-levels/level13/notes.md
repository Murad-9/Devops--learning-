## Goal
The password for the next file is stored in /etc/bandit_pass/bandit14
and can only be read by user bandit 14.For this level, you dont get the
next password, but you get a private ssh key that can be used to log in
to the next level.

## Solution
ls
cat ssh.key
copy and exit 
create own file and paste in the key
chmod 600 the file
ssh -i "filename" bandit14@bandit.labs.overthewire.org -p 2220

## Explanation
In this level there is no password but an sshkey instead.
i copied the sshkey into my own file and changed its permissions
using "chmod 600". This is required because ssh will refuse to use
a keyfile that is readable by others,for security reasons.
After fixing the permissions i logged in with the key.

## Key Lesson
SSH Keys must have restricted permissions to be usable.
