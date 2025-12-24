## Goal
The password for the next level is stored somewhere on the server and 
has the following properties. owned by user bandit 7, owned by group 
bandit 6 , 33bytes in size.

## Solution
ls
find -user bandit7 -group bandit6 -size 33c 2>/dev/null

## Explanation
The "find" command searches through the directories with our filters
applied.Some directories are unreadable so we redirect errors to 
/dev/null to clean the output.

## Password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## Key Lesson
 2>/dev/null hides permission errors
