## Goal
The password for the next level can be retrieved by submitting the 
password of the current level to port 30001 on localhost using SSL
/TLS encryption.


## Solution
openssl s_client localhost:30001
paste password


## Explanation
This level requires connecting to a specific port using SSL encryption
The "openssl,s_client" command opens a secure SSL/TLS connection to 
the service on 'localhost' at port '30001'. Once connected, the pre-
-vious levels password is submitted and the server responds.


## Password
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
