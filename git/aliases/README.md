# Git aliases
## Description
This directory contains some scripts to setup useful git aliases.
## How to setup?
```bash
git config --global alias.$nameOfAlias 'script written within the files in this repository'
```
## What are the aliases?
### 1. br
This alias inherits the functionalities of `git branch` and numbers the branches for further usage.

Example:
```bash
git br # equivalent to git branch

# Result
# 1  * master
# 2    develop
# 3    feature/payment
# 4    fix/payment_crash
```

```bash
git br -d 3 # equivalent to git branch -d feature/payment

# Result:
# Deleted branch feature/payment (was e11f7daae46)
```
### 2. ck
This alias inherits and extends the functionalities of `git checkout`.

Example:
```bash
git br # equivalent to git branch

# Result
# 1  * master
# 2    develop
# 3    feature/payment
# 4    fix/payment_crash
```

```bash
git ck 3 # equivalent to git checkout feature/payment

# Result:
# Switched to branch 'feature/payment'
```

```bash
git ck -d 3 # checkout and then delete the current branch

# Result:
# Switched to branch 'feature/payment'
# Deleted branch current_branch (was 5d8e09aa32).
```
