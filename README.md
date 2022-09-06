# Description

>This shell made by Paul and Joseph is a simple UNIX command interpreter that replicates 
>functionalities of the simple shell (sh). Additional functions are also included. 
>This program was written entirely in C as a milestone project for ALX Africa.


## Abstract
>This Simple Shell repository holds all the requisite for this custom simple shell to run
>Our shell currently handles the executions of executables found in the environmental variable 'PATH'.
>Some of the commands that our custom shell supports include /bin/ls, pwd, env, etc.

#### Some of the allowed functions and system calls
```access```, ```chdir```, ```close```, ```closedir```, ```execve```,```exit```
```_exit```, ```signal```, ```malloc```, ```free```, ```getcwd```, ```wait```, ```write```.


### File Descriptions

> * ```AUTHORS```: include the names of the contributors to this repository.
Paul Walter Adansi and Joseph Tingan
> * ```_realloc.c```: contains a function that reallocates then allocated memory and sets all the values to 0.
> * ```_strings.c```: contains functions that helps in the manipulation os strings including strcat, strcmp, strcpy, st> rd\
> up, strlen.
> * ```builtin_parser.c```: parses the builtin programs.
> * ```cd_handler.c```: include functions that helps to get the current working directory, handles cd when the user does \
> not set any other arguements, navigates to the previous directory when user invokes cd -, and changes the current worki\
> ng directory.
> * ```ctrl_exit.c```: contains functions to display prompt, to ignore spaces before command, to ignore the ctrl-C whene\
> voked, and to handl the shell exit.
> * ```envset_unset.c```: this file contains functions that handles the environment, setting it and also unsetting it.
> * ```execute.c```: this file contains functions to convert sting to token and handles the execution of a file given as \
> input.
> * ```main.h```: handles all the prototypes used in this repository.
> * ```man_1_simple_shell```: This is a manual description of what our shell is and its content and also an example to il\
> lustrate how it works.
> * ```path_handler.c```: this funtion contains functions to get the path of the command, retrive the environment, and re\
> turn full command path.
> * ```print_char.c```: includes the putchar and a print to help print a string.
> * ```read_line.c```: contain functions that reads the characters in standard input.
> * ```shell.c```: this is our main function that displays an prompt and waits for the user to type in a command.


### Shell Usage
* Install
```
(your_terminal)$ git clone https://github.com/DennisWanjeri/simple_shell.git
(your_terminal)$ cd simple_shell
```
* Compile
```
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```
* Usage: non-interactive mode
```
echo "/bin/ls" | ./hsh
```
* Usage: interactive mode
```
(your_terminal)$ ./hsh
```

#### Illustration
```
a#cisfun$ ls -l                                                                                                         total 80
-rw-rw-r-- 1 root root 158  Aug 05 20:43 AUTHORS
-rw-rw-r-- 1 root root 1913 Aug 05 20:52 README.md
-rw-rw-r-- 1 root root 1008 Aug 05 20:54 _realloc.c
-rw-rw-r-- 1 root root 2219 Aug 05 20:58 _strings.c
#cisfun$ echo "simple shell easy!"
simple shell easy!
#cisfun$ exit 98
(your_terminal)$
```
#### Authors
Paul Walter Adansi and Joseph Tingan