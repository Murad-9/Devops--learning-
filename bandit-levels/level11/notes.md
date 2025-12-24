## Goal
The password for the next level is stored in the file data.txt,where
all lowercase(a-z) and uppercase (A-Z) letters have been rotated by
13 positions

## Solution
ls
cat data.txt | tr "n-za-mN-ZA-M" "a-zA-z"

## Explanation
The rot13 cipher shifts the letters forward by 13 places. The "tr" 
commmand translates characters from one set to another.
- "n-za-m" represents the second half of the lowercase alphabet
- "N-ZA-M" represents the second half of the uppercase alphabet
- "a-zA-Z" represents the full normal alphabet.
By Mapping the shifted letters back to the original positions, "tr"
reverses the "rot13"

## Password
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

## Key Lesson
tr translates characters between sets

