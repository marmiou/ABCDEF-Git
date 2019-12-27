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

# What GIT is __**not**__

---

### 1. Git is not Subversion with some added sugar sprinkled in

---

### 2. Git is not expensive network or space wise

---

### 3. Git is not just for hackers or those who fly on airplanes all day to conferences

---

### 4. Git is not hard to set up

---

### 5. Git is not hard to learn

---

### 6. Git is not complex

---

## So...

---

#What __**is**__ GIT?

---

### Git is a VCS 

---

### a.k.a Version Control System

---

### Git is a VCS
- Git keeps track of changes, especially text changes

---

### Git is a VCS
- Git keeps track of changes, especially text changes
- version 1, version 2, version 3

---

### Git is a VCS
- Git keeps track of changes, especially text changes
- version 1, version 2, version 3
- compare versions

---

### Git is a VCS
- Git keeps track of changes, especially text changes
- version 1, version 2, version 3
- compare versions
- see what changed in each version

---

## Git is a __**distributed**__ VCS

---

## Git is a __**distributed**__ VCS

- No central place to store the copy of your project is needed

---

## Git is a __**distributed**__ VCS

- No central place to store the copy of your project is needed
- Different users (or teams) maintain their own repositories

---

## Git is a __**distributed**__ VCS

- No central place to store the copy of your project is needed
- Different users (or teams) maintain their own repositories
- No network connection needed

---

## Git is a __**distributed**__ VCS

- No central place to store the copy of your project is needed
- Different users (or teams) maintain their own repositories
- No network connection needed
- faster

---

# Getting Started

---

#Initializing a git repository

`cd /path/to/your/existing/code`
`git init `

---

## git init 

- Creates a new empty git repository

---

## git init 

- Creates a new empty git repository
- You have an entire repository into your directory

---

## git init 

- Creates a new empty git repository
- You have an entire repository into your directory
- Git does not necessarily need a server to use

---

# Hey!

---

### Where are my changes stored?

![](images/rickMortyFreak.gif)

---

### Cool, huh?

![right](gitTree.png)

---

#Performing our first commit

- Make a change
- Add the change
- Commit the change

`git add <changed file>`
`git commit -m <commit message> `


---

## git add

- Add writes to the repository (in a binary object)
- add creates a new copy of a file

---

## Git commit

- Takes what has been written in the repo and creates a commit object for that
- The commit object has an id (hash)
- The commit object has labels on it (head (where you currently created the object), master (branch))

---