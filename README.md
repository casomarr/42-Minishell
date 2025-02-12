Unix
<a href="https://www.linux.org/"><img src="https://img.shields.io/badge/Linux-CCAC00?style=for-the-badge&logo=linux&logoColor=white" height="25em" alt="Linux"/></a>
C
<a href="https://www.cprogramming.com"><img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" height="25em" alt="C"/></a>

# Minishell

## Goal:
Understand how shells work by creating a simplified version of the Unix shell Bash from scratch.

## Key Features to Implement:
**Command Execution**: Execute basic commands (ls, pwd) using system calls like fork, execve, and wait.
**Redirections**: Handle input/output redirection (>, <, >>).
**Pipes**: Implement piping (|) to connect the output of one command to the input of another.
**Environment Variables**: Manage variables like PATH to locate executables.
**Built-in Commands**: Implement shell-specific commands like cd, echo, export, and exit.
**Signal Handling**: Manage signals like Ctrl+C (SIGINT) and Ctrl+\ (SIGQUIT).

## Challenges:
**Parsing**: Splitting and interpreting user input correctly (handling quotes, spaces, and special characters).
**Memory Management**: Avoiding leaks and managing resources efficiently.
**Error Handling**: Gracefully dealing with errors and invalid input to prevent the program from leaking or crashing.

## Skills Developed:
**System Programming**: Deep understanding of Unix system calls and processes.
**C Programming**: Mastery of memory management, pointers, and data structures.
**Problem Solving**: Designing and implementing a complex system from scratch.

## Installation

To set up this project locally, follow these steps:

1. **Clone the repository to your local machine:**
	```sh
	git clone git@github.com:casomarr/42-Minishell.git
	```

2. **Navigate to the project directory:**
	```sh
	cd 42-Minishell
	```

3. **Compile the project:**
	```sh
	make
	```

4. **Run the shell:**
	```sh
	./minishell
	```

# Usage

Once the shell is running, you can start entering commands. Here are some examples:

- To execute a built-in command:
	```sh
	echo "Hello, World!"
	```

- To set an environment variable:
	```sh
	export MY_VAR="Hello World"
	```

- To run an external command:
	```sh
	ls -l
	```

- To redirect output to a file:
	```sh
	echo "This is a test." > output.txt
	```

- To pipe commands:
	```sh
	cat file.txt | grep "searched_word"
	```

- HEREDOC with variable expansion:
	```sh
	MY_VAR="world"
	cat << EOF
	Hello, $MY_VAR!
	EOF
	```

For more information, refer to the subject.
