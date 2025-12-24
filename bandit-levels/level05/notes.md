## Goal
The password for the next level is stored in a file somewhere in the 
inhere directory and has the following properties.
human-readable,1033 bytes in size,not executable.

## Solution
ls
cd inhere
ls
find -size 1033c
cat ./maybehere07/.file2

## Explanation
The "find" command allows searching through directories using filters
such as size and permissions.By specifying the exact size using "-size"
and "c" for bytes we found the file we needed.

## Password
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
