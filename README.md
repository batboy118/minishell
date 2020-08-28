# minishell

### What is this project about? 

- The objective of this project is for you to create a simple shell. 
- own little bash or zsh. You will learn a lot about processes and file descriptors.

### General instructions

- no memory leak

- Makefile must not relink
- Makefile must at least contain the rules $(NAME), all, clean, fclean and re
- comfile with -Wall, -Wextra -Werror

### Mandatory part

- program name : minishell
- allowed functions : `malloc, free, write, open, read, close, fork, wait, waitpid, wait3, wait4, signal, kill, exit, getcwd, chdir, stat, lstat, fstat, execve, dup, dup2, pipe, opendir, readdir, closedir, strerror, errno`

**shell should be :**

- **Show a prompt** when waiting for a new command
- Search and launch the right executable (based on the PATH variable or by using relative or absolute path) like in bash
- It must implement the builtins like in bash
  - **echo** with option ’-n’
  - **cd** with only a relative or absolute path
  - **pwd** without any options
  - **export** without any options
  - **unset** without any options
  - **env** without any options and any arguments
  - **exit** without any options
- `; `in the command should separate commands like in bash
- `’ `and `"` should work like in bash except for multiline commands
- Redirections `< > “>>”` should work like in bash except for file descriptor aggregation
- Pipes `|` should work like in bash
- `Environment variables ($ followed by characters)` should work like in bash
-  `$?` should work like in bash
- `ctrl-C, ctrl-D and ctrl-\` should have the same result as in bash

### Bonus part

- Redirection `“<<”` like in bash
- wilcard `*` like in bash
- `&&`, `||` with parenthesis for priorities, like in bash

