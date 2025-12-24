## Goal
The password for the next level is stored in the file data.txt next to
the word millionth.

## Solution
ls
wc -l data.txt
grep millionth data.txt

## Explanation
wc -l is a word count command,and the -l option counts only lines.We can
see that "data.txt" has thousands of lines,so searching manunally would
take too long.Instead,we use the "grep" command along with "millionth"
to search through the file efficiently.

## Password
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

