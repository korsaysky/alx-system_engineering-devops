i will add a descciption later
1st task : how to print a message
2d task : if i want to print something with a special character, i use double quotes followed by backsplash
3rd task :The cat command is used to display the contents of a file. In this case, we're using it to display the contents of the /etc/passwd file.
4th : the cat command to display the content of multiple files. the space between the two files it's equivalent to = and
5th : This script simply calls tail with the -n 10 option, which specifies that the last 10 lines of the file should be displayed. The file path /etc/passwd is provided as an argument to tail to specify the file to operate on
5d : This script displays the first 10 lines of the /etc/passwd file. The script achieves this by calling the head command with the -n 10 option, which specifies that the first 10 lines of the file should be displayed. The file path /etc/passwd is provided as an argument to head to specify the file to operate on.
6th : The first line specifies that the script should be run with bash.
The head command is used with the -n 3 option to print the first three lines of the file iacta.
The tail command is used with the -n 1 option to print the last line of the output produced by head -n 3.
The result is that the third line of the file iacta is printed to the standard output
8 : The first line #!/bin/bash is the shebang line that specifies the interpreter that will be used to execute the script.

The second line ls -la > ls_cwd_content uses the ls command with the -la option to list all files and directories in the current working directory in long format (including file permissions, ownership, size, and modification time), and redirects the output to a file named ls_cwd_content.

The > operator used in the command above is called output redirection, and it redirects the output of the ls -la command to a file instead of printing it on the terminal.

If the file ls_cwd_content already exists, the above command overwrites its contents, and if it doesn't exist, the command creates it.
task 9: tail -n 1 iacta >> iacta: This command appends the last line of the file 'iacta' to the end of the same file. The 'tail' command prints out the last 'n' lines of a file, where 'n' is specified by the '-n' flag. In this case, '-n 1' means to print the last line of the file. The '>>' operator is used for redirection and appends the output of the 'tail' command to the end of the same file 'iacta'.

task 10 : #!/bin/bash: This line is known as the "shebang" and is required at the beginning of every bash script. It tells the system that this file is a bash script and that it should be run with the bash interpreter.

find .: This command searches for files and directories recursively in the current directory and all its subfolders.

-type f: This option specifies that we're only interested in regular files, not directories or other types of files.

-name "*.js": This option specifies that we're only interested in files with a ".js" extension.

-delete: This option specifies that we want to delete the files that match the previous options.

task 11: #!/bin/bash: specifies the shell to be used for the script
find . -type d: searches for directories in the current directory and subdirectories
| : then 
wc -l: counts the number of directories and subdirectories found by the find command
mindepth 1 option ensures that the current directory is not included in the search 

task 12 : The second line uses the ls command with the -t option, which sorts the files in the current directory by modification time, with the newest files appearing first. The output of ls is then piped to head, which displays only the first 10 lines .

task 13 : 
 sort is used to sort the words in alphabetical order.
uniq -u prints only the unique lines that appear exactly once. The -u option tells uniq to only print the lines that occur once in the sorted input.
To run the script, you can provide the list of words as input using standard input (stdin) like this: cat README.md | ./13-unique

task 14,15,16 : i will add descrp later

task 17 : grep -v "bin" /etc/passwd: This line uses the grep command to search for lines in the /etc/passwd file that do not contain the pattern "bin". The -v option is used to invert the match, meaning that lines that do not contain the pattern will be displayed. The output of this command will be all the lines in /etc/passwd that do not contain the pattern "bin"

task 18 : grep is a command-line utility that searches for patterns in text.
"^[[:alpha:]]" is a regular expression that matches all lines starting with a letter. The caret (^) is used to match the beginning of a line, and [[:alpha:]] matches any alphabetic character.

task 19 : The tr command is used to perform the character substitution. The first argument passed to the tr command specifies the set of characters to be replaced, and the second argument specifies the set of characters to replace them with. In this case, we specify that 'A' should be replaced with 'Z' and 'c' should be replaced with 'e'. The script reads input from standard input and writes the modified output to standard output.


