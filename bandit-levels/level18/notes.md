## Goal
The password for the next level is stored in a file readme in the home
directory.Unfortunatley,someone has modified .bashrc to log you out 
when you log into with SSH

## Solution
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme

## Explanation
The bandit18 shell is configured to disconnect immediately. By adding
The commmans "cat readme" to the ssh command, the ssh executes the 
command before the shell starts.This allows the contents of "readme"
to be printed before disconnection.

## Password
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
