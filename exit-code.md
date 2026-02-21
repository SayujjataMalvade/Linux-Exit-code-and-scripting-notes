# Linux Exit Codes

Every Linux command returns an exit code after execution.
Exit codes help identify whether a command succeeded or failed.

## Basic Rule
- 0  → Success
- Non-zero → Failure

## Common Exit Codes

| Exit Code | Meaning |
|---------|--------|
| 0 | Command executed successfully |
| 1 | General error |
| 2 | Misuse of shell built-in |
| 126 | Command found but not executable |
| 127 | Command not found |
| 128+N | Process terminated by signal |

## Important Exit Codes (DevOps Focus)

- 127 → Missing command / dependency
- 126 → Permission issue
- 130 → Process interrupted (Ctrl+C)
- 137 → Process killed (OOM / SIGKILL)
- 143 → Graceful termination (SIGTERM)

Exit codes give the *direction* of the issue.
Logs give the *details*.
