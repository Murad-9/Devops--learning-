## Goal
The password for the next level is stored in the file data.txt,which is
a hexdump of a file that has been repeatedly compressed.

##  Solution
mkdir /tmp/random12
cp data.txt /tmp/random12
file data.txt
xxd -r data.txt > decrypt.txt
file decrypt.txt
mv decrypt.txt decrypt.gz
gzip -d decrypt.gz
file decrypt
bzip -d decrypt
file decrypt.out
mv decrypt.out decrypt.gz
gzip -d decrypt.gz
file decrypt
tar -x -f decrypt
ls
tar -x -f data5.bin
ls
file data6.bin
bzip -d data6.bin
ls
file data6.bin.out
tar -x -f data6.bin.ou
ls
file data8.bin
mv data8.bin data8.gz
gzip -d data8.gz
ls
file data8
cat data8


## Explanation
This level involved a file that had been compressed multiple times
using different formats.First,a directory was created in 
/tmp.The file was copied into our directory and converted back from the
hexdump using " xxd -r" the ">" was used to redirect output into a new
file.Redirecting allows us to save the decoded result as a file so it 
can be proccessed further.The file was then repeatedly checked using 
the "file" command to identify its compression type.
- gzip -d for gzip files
- bzip2 -d for bzip files
- tar -x -f for tar archives
the process was repeated until the final readable file was extracted.

## Password
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

## Key Lesson
use a new/temporary directory to proccess safely
use > so you can save it to a file for further processing 
use "file" to see which format you need to decompress.


