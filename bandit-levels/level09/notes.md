## Goal
The password for the next levle is stored in the file data.txt in one
of the few human-readable strings, preceeded by several "=" characters.

## Solution 
ls
strings data.txt | grep ===

## Explanation
"Strings" extracts human-readable text from a binary or non text file.
Piping the output into "grep" allows filtering for lines containing the
pattern "===",which is part of the password format.

## Password 
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

## Key Lesson
Strings is useful for extracting readable text from binary files. 
