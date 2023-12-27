# Helpful reminders and todos

## wget

Download all URLs stored in a text file to a specific directory:

```bash
wget --directory-prefix path/to/directory --input-file URLs.txt
```

## github requests

[get list of files in a repo (and some metadata)](https://api.github.com/repos/[USER]/[REPO]/git/trees/[BRANCH]?recursive=1)
