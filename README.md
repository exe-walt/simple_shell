# Description

>This shell made by Paul and Joseph is a simple UNIX command interpreter that replicates 
>functionalities of the simple shell (sh). Additional functions are also included. 
>This program was written entirely in C as a milestone project for ALX Africa.

# Simple Shell
Simple Shell is a project for students at Holberton School. The project test everything we have learned about the C pro\
gramming language and our skills for work as a team and planning for a long term project.
### Description
The Simple Shell is a simple UNIX command interpreter written in C. The program runs based on bash commands obtained fr\
om the input stream by the user, the respective command typed by the user in executed as if in a UNIX shell.
### Requirements
- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 14.04 LTS
- Your C programs and functions will be compiled with gcc 4.8.4 using the flags -Wall -Werror -Wextra and -pedantic
- All your files should end with a new line
- A README.md file, at the root of the folder of the project is mandatory
- Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
- Your shell should not have any memory leaks
- No more than 5 functions per file
- All your header files should be include guarded
- Use system calls only when you need to (why?)
### Compilation
All of the ``.c`` files along with a main.c file are to be compiled with ``gcc 4.8.4`` on Ubuntu 14.04 LTS with the fla\
gs ``-Wall Werror`` ``-Wextra`` and ``-pedantic.``
The files will be compiled this way:
- ``gcc -Wall -Werror -Wextra -pedantic *.c -o hsh``

### Execute
```{bash}
$ ./hsh
```

### Usage
The shell works like this in interactive mode:

```{bash}
($) ls -l
total 72
-rw-rw-r-- 1 vagrant vagrant   343 Sep 6 10:02## Simple Shell

### Synopsis
15
> On this Simple Shell repository it holds all the code necessary for
16
> our custom simple shell to run. Our shell currently handles the executions
17
> of executables found in the environmental variable PATH.
18
> Some of the commands that our shell supports include /bin/ls, pwd, env, etc.
19

20
#### Some of the allowed functions and system calls
21
```access```, ```chdir```, ```close```, ```closedir```, ```execve```,```exit```
22
```_exit```, ```signal```, ```malloc```, ```free```, ```getcwd```, ```wait```, ```write```.
23

42
### Shell Usage
43
* Install
44
```
45
(your_terminal)$ git clone https://github.com/JuskingA/simple_shell.git
46
(your_terminal)$ cd simple_shell
47
```
48

* Compile
49
```
50
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
51
```
52
* Usage: non-interactive mode built_in.c
-rw-rw-r-- 1 vagrant vagrant   850 Sep 10 10:02 error.c
-rw-rw-r-- 1 vagrant vagrant   555 Sep 10 10:27 execute_line.c
-rw-rw-r-- 1 vagrant vagrant   305 Sep 10 10:46 _getenv.c
-rwxrwxr-x 1 vagrant vagrant 14563 Sep 10 10:57 hsh
($)
```

* Usage: non-interactive mode built_in.c
-rw-rw-r-- 1 vagrant vagrant   850 Sep 10 10:02 error.c
-rw-rw-r-- 1 vagrant vagrant   555 Sep 10 10:27 execute_line.c
-rw-rw-r-- 1 vagrant vagrant   305 Sep 10 10:46 _getenv.c
-rwxrwxr-x 1 vagrant vagrant 14563 Sep 10 10:57 hsh
($)
```
```{bash}
($) pwd
/home/vagrant/simple_shell
($)
```
```{bash}
($) exit
$
```
The shell works like this in non-interactive mode:
```{bash}
$ echo "/bin/ls" | ./hsh
built_in.c      _getenv.c    man_1_simple_shell  shell.c         split_line.c
error.c         hsh          mini_shell          shell.h         useful_func.c
execute_line.c  list_path.c  README.md           special_case.c  _which.c
$
```
```{bash}
$ echo "///////bin/////ls" | ./hsh
built_in.c      _getenv.c    man_1_simple_shell  shell.c         split_line.c
error.c         hsh          mini_shell          shell.h         useful_func.c
execute_line.c  list_path.c  README.md           special_case.c  _which.c
$
```
```{bash}
$ echo "non-interactive" | ./hsh
./hsh: 1: non-interactive: not found
$
```
### Built-ins
The simple shell has support for the following built-in commands:
Command   |   Definition
---------------- | ------------------ |
env | Prints the environment
exit | Exits the shell

#### Authors
Paul Walter Adansi and Joseph Tingan
