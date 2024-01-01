# Bourne Again SHell prompt

`machine-name:current-working-directory$`

~ means home
$ means not the root user

We can type in commands at the shell

The shell parses the command

- splitting it by whitespace,
- runs the program (first word),
- supplying each subsequent word as an argument
  - argument that contains spaces or other special characters
    - either quote the argument with ' or "
    - or escape just the relevant characters with \

The shell is a programming environment with variables, conditionals, loops, and functions.

`date` prints the current date and time.

`echo` prints out its arguments.

`$PATH` is an environment variable that lists which directories the shell should search for programs when it is given a command.

`which` find out which file is executed for a given program name

Bypass $PATH by giving the path to the file we want to execute.

Path

- delimited list of directories
- separated by / on Linux and macOS and \ on Windows
- the path /
  - linux and macOS
  - “root” of the file system
  - absolute path
    - starts with /
  - relative path
    - relative to the current working directory

`pwd` print working directory
`cd` change current working directory

`.` current directory
`..` parent directory
  
`ls` list files in current directory

`~` home directory

`-` flags with values modify command behavior

`-h` or `--help` flag will print some help text

`cd -` previous directory

`mv` rename, move a file

- two arguments
  - renames the first arg as the second (file name) or,
  - moves moves first arg to the second (directory)

`cp` copy a file or directory
`cp [options] source destination`
`cp file.txt backup/` copy a file from one location to another
`cp file1.txt file2.txt backup/` copy multiple files 
`cp -r mydirectory/ backup/` copy an entire directory and its contents
 Be cautious with the -r option, as it can overwrite files and directories.

`mkdir` make a new directory

`man` takes as an argument the name of a program, and shows you its manual page

`q` to exit

`ctr l` clears terminal

Connecting programs

- input stream
  - program reads input from input stream
  - default keyboard

- output stream
  - sends data out of the program
  - default screen

`< file` rewire the input of this program to be the contents of a file

`> file` rewire the output of the preceding program into this file

`cat` prints the context of a file

`>>` append

`|`

- take the output of the program to the left and make it the input to the program on the right.
- “chain” programs such that the output of one is the input of another

`#` mean run as root

`touch` create new file
