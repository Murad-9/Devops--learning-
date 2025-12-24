## Goal
The password for the next levl can be retrieved by submitting the 
password of the current level to port 30000 on localhost.

## Solution 
cd /etc/bandit_pass/bandit14 
cat bandit14
copy password
nc localhost 30000
paste password

## Explanation
The "nc" (netcat) command is used to open a raw TCP connection to a
specific port on a local machine.Once connected, the service waits for 
input.By pasting the current password, the service verifies it and re-
-turns the next password.

## Password
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo


