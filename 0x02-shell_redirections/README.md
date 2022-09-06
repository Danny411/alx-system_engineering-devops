#!/bin/bash
This is a new project that talks about new characters amd commands for shell redirections and filters without the use of "AWK"  language

echo Hello, World ...  a script that prints “Hello, World”, followed by a new line to the standard output 

echo ""(Ôo)'"  ..... a script that displays a confused smiley "(Ôo)' 

cat /etc/passwd  .... a script that displays the content of the /etc/passwd file 

cat /etc/passwd /etc/hosts .... A script that displays the content of /etc/passwd and /etc/hosts 

tail /etc/passwd  .... a script that dsplay the last 10 lines of /etc/passwd 

head /etc/passwd ..... a script that display the first 10 lines of /etc/passwd 

head --lines=3 iacta | tail --lines=1  ..... a script that displays the third line of the file


echo "Best School" >> "\\*\\\\'\"Best School\"\\'\\\\*\$\\?\\*\\*\\*\\*\\*:)"  ..... a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:)


ls -la > ls_cwd_content .... a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.


echo -en "" | tail --lines=1 iacta >> iacta .... A script that duplicates the last line of the file iacta(ie The file iacta will be in the working directory).


find . -name '*.js' -type f -delete  ...a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders


find -mindepth 1 -type d | wc -l  ....  a script that counts the number of directories and sub-directories in the current directory.(ie The current and parent directories should not be taken into account, Hidden directories should be counted)


ls -t | head  .... A script that displays the 10 newest files in the current directory.(ie One file per line, Sorted from the newest to the oldest)


sort | uniq -u .... a script that takes a list of words as input and prints only words that appear exactly once. (Ie Input format: One line, one word, Output format: One line, one word, Words should be sorted)


grep -i root /etc/passwd  .... a script that displays lines containing the pattern "root" from the file /etc/passwd


grep -i bin /etc/passwd | wc -l  .... a script that display the number of lines that contain the pattern “bin” in the file /etc/passwd


grep -iA 3 root /etc/passwd ..... a script that display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd


grep -iv bin /etc/passwd ..... a script that display all the lines in the file /etc/passwd that do not contain the pattern “bin”.


grep -i "^[a-z]" /etc/ssh/sshd_config  ..... a script that isplay all lines of the file /etc/ssh/sshd_config starting with a letter. (ie include capital letters as well 

tr Ac Ze  ..... a script that replace all characters A and c from input to Z and e respectively 

tr -d cC  ..... a script that removes all letters c and C from input 

rev ..... a command that reverse it inputs


cut -d':' -f1,6 /etc/passwd | sort .....a script that displays all users and their home directories, sorted by users.(ie Based on the the /etc/passwd file


find . -empty -printf "%f\n"  .....a command that finds all empty files and directories in the current directory and all sub-directories.
• Only the names of the files and directories should be displayed (not the entire path)
• Hidden files should be listed
• One file name per line
• The listing should end with a new line
• You are not allowed to use basename, grep, egrep, fgrep or rgrep


find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f ..... A script that lists all the files with a .gif extension in the current directory and all its sub-directories.
• Hidden files should be listed
• Only regular files (not directories) should be listed
• The names of the files should be displayed without their extensions
• The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay)
• One file name per line
• The listing should end with a new line
• You are not allowed to use basename, grep, egrep, fgrep or rgrep



cut -c 1 | tr -d '\n' | sort  ..... a script that decodes acrostics that use the first letter of each line.
• The ‘decoded’ message has to end with a new line
• You are not allowed to use grep, egrep, fgrep or rgrep


tail -n +2 | cut -f1 | sort | uniq -c |sort -nr | head -11 | tr -s ' ' | cut -d' ' -f3 ..... A script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
• Order by number of requests, most active host or IP at the top
• You are not allowed to use grep, egrep, fgrep or rgrep

