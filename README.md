# TO REPRODUCE

```bash
yarn patch-task-hasher

# Run once.
nx run-many --all -t hello

# Run again, no cache hits.
nx run-many --all -t hello
```
