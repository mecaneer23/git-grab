# Git Grab

`git clone`, but without `git`.

## What is Git Grab?

`git-grab` emulates `git clone`, grabbing all of the files from a provided git repository. However, it ignores all git history and doesn't grab the git files.

## Installing

### With `wget`

```bash
wget --output-document ~/.local/git-grab https://raw.githubusercontent.com/mecaneer23/git-grab/main/git-grab
```

### With `curl`

```bash
curl -f https://raw.githubusercontent.com/mecaneer23/git-grab/main/git-grab -o ~/.local/git-grab
```

## Running

Usage: `git-grab [options] url [path]`

```bash
# example
git-grab https://github.com/mecaneer23/git-grab
```

### What can `url` be?

Currently, repositories from the following sites are supported.

- [github.com](https://github.com)

Make sure to include the full url, such as [https://github.com/mecaneer23/git-grab](https://github.com/mecaneer23/git-grab).

### Options

| Option           | Default | Description                                                       |
| ---------------- | ------- | ----------------------------------------------------------------- |
| --dependency, -d | `wget`  | Takes in one of (`wget`, `curl`). Uses this program to get files. |

### Path

`path` provides a way to use a custom repository name, other than the default.

Installing the `git-grab` repository in a folder called `grab`

```bash
git-grab https://github.com/mecaneer23/git-grab grab
```
