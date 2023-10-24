# TO REPRODUCE

```bash
# Disable nx daemon, force usage of InProcessTaskHasher
export NX_DAEMON=false

# Copy our patched task hasher with print statements.
yarn patch-task-hasher

# Run once.
nx run-many --all -t hello

# Run again, no cache hits.
nx run-many --all -t hello
```
