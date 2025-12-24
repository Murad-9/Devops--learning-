## Goal
There is a setuid binary in the homedirectory that does the following:
it makes a connection to localhost on the port you specify as a comm-
-andline argument. it then reads a line of text from the connection and
compares it to the password in the previous level.If the password is 
correct,it will transmit the next password.

## Solution
nc -l localhost 4444
./suconnect 4444
paste password from previous level

## Explanation
suconnect is a program that connects to a TCP port on localhost. It 
expects a listener on the other end to recieve the current password.
once the correct password is sent,suconnect sends back the password
for the next level. This works because TCP connections allow two 
programs to send and recieve text.

## Password
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
