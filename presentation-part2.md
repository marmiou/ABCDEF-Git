footer: © Epignosis LLC
slidenumbers: true

> ABCDEF GIT
-- An in depth intro to GIT

---

# Agenda

- What is not GIT
- What is GIT
- Getting started
- Git concepts and architecture
- Making changes to files

---

# Agenda

- Undoing changes
- Ignoring files
- Navigating the commit tree
- Branching
- Merging Branches

---

# Agenda

- Stashing
- Remotes
- Tips and tricks
- Resources

---

# Making changes to files

---

> Repetition is the mother of learning
--Zig Ziglar

---

## Making changes to files

`git add`
`git diff --staged`
`git commit -m "<message>"`

---

## Deleting files

---

## Deleting files

`rm -rf /path/to/file`
`git add /path/to/file`
`git commit -m "<message>"`

---

## Deleting files

`git rm /path/to/file`
`git commit -m "<message>"`

---

## Moving and Renaming files

---

## Renaming files

`mv /path/to/file /path/to/new-file`
`git add /path/to/new-file`
`git rm /path/to/file`
`git commit -m "<message>"`

---

## Renaming files

`git mv /path/to/file /new/path/to/new-file`
`git commit -m "<message>"`

---

## Moving files

---

## Moving files

`mv /path/to/file /new/path/to/file`
`git add /new/path/to/file`
`git rm /path/to/file`
`git commit -m "<message>"`

---

## Moving files

`git mv /path/to/file /new/path/to/file`
`git commit -m "<message>"`

---

![130%](images/undo.gif)

---

# Undoing changes

---

## Undoing changes

- Changes in the working directory
- Changes in the staging index
- Changes in the repository

---

## Undoing changes in the working dir

`git checkout -- /path/to/file`
`git clean -n`
`git clean -f`
`git clean -dn`
`git clean -df`

---


## Un-staging files

`git reset HEAD /path/to/file`

---

## Really? But where can this be useful?

![](images/alice.gif)

---

![](images/alice.gif)

---

### Mumble mumble...

---

### Perhaps you forgot __**all the changes**__ you wanted to commit in a file...

---

### ...and you __**don't want to mess**__ history with multiple commits?

---

## Amending commits

---

### Amending commits

`git commit --amend`
`git commit --amend --no-edit`

---

### Amending commits

- You need to modify commit message
- You need to combine staged changes with the latest commit

---

### But __**remember**__!

---

### Avoid amending a commit that other developers have based their work on. 

---

### Changing history on a remote is a __**bad practice**__

---

### And __**remember**__!

---

### Not a good idea to amend older than the latest commits!

---

## Retrieving old versions

---

## Retrieving old versions

`git checkout -- <hash-of-previous-commit> /path/to/file`

---

## Retrieving old versions

- You need to retrieve a previous version of a file
- The change will be applied into the staging area
- A good practice if you want to revert a particular change in previous SHA

---

## Reverting commits


---
## Using Reset