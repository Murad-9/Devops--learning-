# Bandit level 1 - 2 

## Goal
The password for the next level is stored in a file called "-" 
located in the home directory

## Solution
ls 
cat ./-

## Explanation
Normally "-" is treated as an option by commands,using just "cat
alone will not work, so we need to prevent that.
using "cat ./" tells the system to read the file named "-" in the
current directory.

## Password
263JGJPfgU6LtdEvgfWU1XP5yac29mFx 

## Key Lesson
"./" is used to explicitly refrence files in the current directory,
especially when filenames start with special characters.
