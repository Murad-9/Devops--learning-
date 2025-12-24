## Goal
The password for the next level is stored in the file data.txt,which 
contains base64 encoded data

## Solution
ls
cat data.txt
base64 -d data.txt

## Explanation
Base64 is an encoding scheme used to represent binary data as readable
text. The "-d" option decodes base64-encoded data back into its origi-
-nal form. By decoding the file, our hidden password is revealed.

## Password
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

## Key Lesson
base64 is encoding not encryption.Purpose: make data readable or
transferable.
