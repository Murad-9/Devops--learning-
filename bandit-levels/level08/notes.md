## Goal
The password for the next level is stored in the file data.txt and is
the only line of text that occurs only once.

## Solution
ls
sort data.txt | uniq -u

## Explanation
Sort arranges all the lines in the file so that identical lines are 
grouped together. uniq -u then prints only the line that appears once.
By combining these commands with a pipe "|" , the line containing the
password appears.

## Password
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

## Key Lesson
Sort is often required before using uniq
Pipes allow the output of one command to be used as input for another
