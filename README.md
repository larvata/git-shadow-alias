git-shadow-alias
=====================

This bash script builds a alias script to helps you maintain multi-repo in same folder.
Change target repo without commands set git work-dir.
Only use your command-alias replace git command to manage repos.
Each repo use .gitignore themself.

## Quick Guide

#### install

`bash git-shadow install`

#### create alias bash script

`git shadow create <git-repo> <command-alias>`

#### load alias

`. .gitkeep/alias`

#### manage < git-repo > with < command-alias >

```
<command-alias> init
<command-alias> add *
<command-alias> status
```

## Command List

**git shadow install**
:   install this script to your ~/bin

**git shadow uninstall**
:   delete this script from your system

**git shadow create < git-repo > < command-alias >**
:   create alias

**git shadow rebuild**
:   reset command-alias for your current repos.
    you should run this command when move the project directory

**git shadow list**
:   list all command-alias exist

## .gitkeep

Git shadow alias use .gitkeep for mantains command-alias and .gitignore. 
Save your .gitignore to .gitkeep and named < git-repo >.gitignore. 
This script will copy currect .gitignore to your current git work-dir.








