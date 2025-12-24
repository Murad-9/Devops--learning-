## Goal
The credentials for the next level can be retrieved by submitting the
password of the current level to a port on localhost in the range of
31000-32000.First find out which of these ports have a server listening
on them.Then find out which of those speak SSL/TLS and which dont.There
is only 1 server that will give the next credentials.

## Solution
nmap -sV localhost -p 31000-32000
ncat localhost --ssl 31790
paste password
copy contents of key into own file
chmod 600 own file
ssh -i to log into next level

## Explanation
nmap -sV scans ports from 31000-32000 and detects which services are
running and wether they use SSL.From the scan results we identify the 
SSL enabled ports.ncat localhost --ssl 31790 connects securley to the 
service using SSL, allowing us to send the current password.The ser-
-vice returns an SSH private key which we then put into our own file,
chmod 600 the file and log in with ssh -i.
