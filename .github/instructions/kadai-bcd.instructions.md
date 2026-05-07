---
applyTo: "kadai-bcd/**"
---

# kadai-b

**Problem statement:** Extend `myexec` from kadai-a to read commands from stdin instead of
command-line arguments, implementing a minimal shell-like loop.

**Requirements:**

- Use `fork(2)` to create the child process.
- Use `execve(2)` to execute the specified program — library wrappers like `system(3)` or
  `execvp(3)` are not allowed.
- One can assume the program path is an absolute path.
- The child process must inherit the parent's environment variables.

**Optional requirements:**

- Implement `PATH` expansion to support specifying programs with relative paths.

# kadai-c

**Problem statement:** Extend the shell from kadai-b to support redirection and pipes.

**Requirements:**

- Support stdin redirection (`<`) and stdout redirection (`>`).
- Support a single pipe (`|`) between two commands.
- stderr redirection is not required.
- Multiple redirections or multiple pipes are not required.

# kadai-d (optional)

**Problem statement:** Extend the shell from kadai-c with append redirection and support for
combinations of multiple redirections and pipes.

**Requirements:**

- Support append output redirection (`>>`).
- Support multiple pipes chained together (e.g. `cmd1 | cmd2 | cmd3 | cmd4`).
- Support combinations of redirection and multiple pipes (e.g. `cmd1 < infile | cmd2 | cmd3 > outfile`).
