# Linux Signals

Signals are messages sent by the OS to processes.

## Common Signals

| Signal | Number | Description |
|------|--------|-------------|
| SIGINT | 2 | Interrupt (Ctrl+C) |
| SIGKILL | 9 | Force kill |
| SIGTERM | 15 | Graceful termination |

## Signal-Based Exit Codes

Exit code = 128 + signal number

Examples:
- SIGINT (2)  → 130
- SIGKILL (9) → 137
- SIGTERM (15) → 143

These exit codes are commonly seen in Docker, Kubernetes, and CI/CD pipelines.
