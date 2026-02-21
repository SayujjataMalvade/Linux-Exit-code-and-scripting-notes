# How DevOps Engineers Use Exit Codes

## CI/CD Pipelines
- Exit code 0 → next stage runs
- Non-zero → pipeline stops

## Cron Jobs
- Exit codes indicate success or failure
- Used for alerting and monitoring

## Containers & Kubernetes
- 137 → OOMKilled or force kill
- 143 → Pod terminated gracefully

## Debugging Approach
1. Check exit code
2. Identify category of issue
3. Check logs for details
