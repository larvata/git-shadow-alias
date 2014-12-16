git-shadow-repos
=====================

This bash script can manage multiple git repos in same git dir.
I use this script mantain .net website. One repo for source control, and one for deploy(only contains complined files and resource file).

## Quick Guide

#### install

`./git-shadow install`

#### init shadow repo

`git shadow init <shadow-repo>`

#### manage repo with git-shadow

```
git shadow add *
git shadow status
...
```

#### restore project from remote repo
```
git clone <url>
cd <target-project-dir>
git shadow clone <git-repo> <shadow-repo-url>
```

## Usage
```
Install: ./git-shadow install
  Usage: git shadow [shadow command]
     or: git shadow [git command]

Git shadow commands:
install             install this script
uninstall           remove this script from system
init [repo]       init shadow repo and set as default
clone [repo] [url]  create shadow repo from remote
current [repo]      set default repo
current             list all shadow repos
```

## Known Issues
- [Windows Only] you should reinstall `./git-shadow install` to update this script manually while you get new version.







