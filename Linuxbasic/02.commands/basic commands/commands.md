How to check your current location ?
-> pwd

How to display name of current logged in user ?
-> whoami

How to check system date or time ?
-> date
or date %D

How to display files and directory present in current location ?
-> ls
ls -lt

How to clear linux terminal ?
-> clear

How to display content of a file on terminal ?
-> cat <file>

How to read file and search for a word ?
-> less <file>

How to view content of a file page by page ?
-> more <file>

How to create a file in linux ?
touch <file_name>

How to delete a file in linux ?
rm <file_name>

How to edit a file in linux ?
-> vi <file_name>
or nano <file_name>

How to create a dictinoray/folder in linux ?
-> mkdir <dir_name>

How to delete a dictionary/folder in linux ?
-> rmdir <dir_name>
rm -rf <dir_name>

How to change path or move to another folder in education ?
-> cd /path/folder
cd ..

How to copy and paste a file from one folder to another in linux ? 
-> cp <file>/des +/path

How to cut-paste a file from one folder to another in linux ?
-> mv <file> /des /path

How to rename a file in linux ?
-> mv fileA fileNewName

How to read or display top 5 lines from a file in linux ?
-> head -5 file

How to read or display bottom 5 lines from a file in linux ?
-> tail -5 file

How to SORT the content from a file in linux ?
-> sort file
sort -r file

How to display unique content from a file in linux ?
-> sort file | uniq

A file has 9 lines.
How to split this file in 3 different files in linux ?
-> split -l 3 file

How to search a word and display matching content from a file in linux ?
-> grep "word" file

How to search multiple words and display matching content from a file in linux ?
-> grep "word 1|word 2" file

How to use wildcards in linux ?
*[]{}
-> ls file *
touch file{1...5}

How to shuffle content of a file in linux ?
-> shuf file

How to count no. of lines in a file in linux ?
-> wc -l file

How to check if two files are indentical or not in linux ?
-> cmp fileA fileB

How to compare and display difference between two file in linux ?
-> diff -u fileA fileB

How to find a file in linux ?
-> find/path/-name<file>