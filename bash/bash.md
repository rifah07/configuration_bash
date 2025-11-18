# Bash Scripting Introduction

## Introduction to Bash

Bash (Bourne Again SHell) is a Unix shell and command language used for interacting with the operating system via a command-line interface. Bash scripting automates repetitive tasks, manages system operations, and enhances productivity by writing sequences of commands in a file (script). It is widely used by developers, system administrators, and DevOps engineers for scripting on Linux and Unix-like systems.

Key features of Bash scripting:
- Scripts begin with a "shebang" `#!/bin/bash` to specify the shell interpreter.
- Supports variables, control structures (if, loops, case), functions, and arrays.
- Enables input/output handling, command substitution, and argument parsing.
- Allows automation of tasks such as backups, program execution, and system monitoring.

## Common Bash Questions and Answers

1. **What is Bash?**  
   Bash is a command-line shell and scripting language used on Linux and Unix-like systems to execute commands and automate tasks.

2. **How do you create and run a Bash script?**  
   - Create a file with a `.sh` extension.
   - Write your script starting with `#!/bin/bash`.
   - Make it executable using `chmod +x filename.sh`.
   - Run it with `./filename.sh`.

3. **What are variables in Bash?**  
   Variables store data and can be assigned without spaces:  

    ```
    name="John"
    echo $name
    ```


4. **Explain control structures in Bash.**  
Bash supports `if-else`, `for`, `while`, and `case` statements for conditional execution and loops.

5. **How do you pass arguments to a Bash script?**  
Arguments are accessed using `$1`, `$2`, ..., `$@` for all arguments.

6. **What is the shebang (#!) in a Bash script?**  
It specifies the script interpreter; typically `#!/bin/bash` tells the system to run the script with Bash.

7. **How do you read user input in Bash?**  
Using the `read` command:  
```
    echo "Enter your name:"
    read name
    echo "Hello, $name"
```

8. **What are functions in Bash?**  
Functions group commands for reuse:  
```
    function greet() {
        echo "Hello, $1"
    }
    greet "World"
    ```


9. **How do you handle errors in Bash scripts?**  
By checking exit status `$?` of commands and using `set -e` to exit on errors.

10. **What are some common Bash commands?**  
 Examples: `echo`, `cat`, `grep`, `chmod`, `ls`, `ps`, `kill`, `sed`, `awk`.

---
