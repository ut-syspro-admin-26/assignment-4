---
applyTo: "kadai-a/**"
---

**Problem statement:** Create a C program named `myexec` that executes a given command as a child
process. Usage: `myexec <program_path> [args...]`. Example: `$ ./myexec /bin/ls -l /var`

**Requirements:**

- Use `fork(2)` to create the child process.
- Use `execve(2)` to execute the specified program — library wrappers like `system(3)` or
  `execvp(3)` are not allowed.
- One can assume the program path is an absolute path.
- The child process must inherit the parent's environment variables.
