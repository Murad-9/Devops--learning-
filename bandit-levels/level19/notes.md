## Goal
To gain access to the next level,you shoulduse the setuid binary in the
home directory.Execute it without arguments to find out how to use it.
The password for this level can be found in the usual place 
/etc/bandit_pass.

## Solution
./bandit20-do cat /etc/bandit_pass/bandit20

## Explanation
bandit20-do is a setuid binary code owned by bandit20.When you execute
it,the command runs with bandit20's permissions not yours.By providing
cat /etc/bandit_pass/bandit20 as an argument, the binary executes cat 
as bandit20 and allows access to the file.

## Password
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## Key Lesson
Setuid binaries run with the owners permissions.
