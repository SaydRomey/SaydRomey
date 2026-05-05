
# Git(hub) Notes

> Guides, notes, commands, etc...

## Basic Info

### 1. Install git: `sudo apt-get install git`

### 2. Configure git:
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

### 3. Generate and add **SSH Key**
- Generate: 
`ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`

- Add the SSH key to your github account:
  `"Settings">"SSH and GPG keys">"New SSH key"`
			(paste the key and save it)

> [!NOTE] More Info  
> <details><summary>Click for more info on -> <code>ssh-keygen -t rsa -b 4096 -C "your_email@example.com"</code></summary>
>
> - `-t`: This option specifies the type of key to create. 
>
> - `rsa`: **RSA** *(Rivest–Shamir–Adleman)* is an algorithm used for key generation.  
>   **RSA** is one of the most common algorithms for generating **SSH keys** 
>   and is known for its security and efficiency.
>
> - `-b`: This specifies the number of bits in the key, affecting the security of the key.
>
> - `4096`: Choosing 4096 bits makes the key stronger 
>   and more secure than the more commonly used 2048 bits. 
> 
>   This number indicates the size of the key, 
>   with a larger size providing higher security 
>   but potentially taking more time to generate and use.
> 
> - `-C`: This option is for a comment.
>   It's not part of the key itself, but it's used to identify the key.  
>   The comment can be any string, but it’s common to use your email for easy identification.
> 
> - `"your_email@example.com"`: This is the comment you've added to the key.  
>   It's especially useful if you have multiple keys and need to distinguish between them.
> 
> In summary, the command `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`  
> is used to generate a new **RSA SSH key of 4096 bits with your email as a comment**. 
>
> This creates a secure key that can be added to services like **GitHub** for authentication.
>
> </details>

---

### 4. Clone the repository from the github URL:
```bash
git clone <repository-url> [foldername]
```

### 5. Work on the project:

- Navigate into the repository's directory:
```bash
cd <repository-name>
```
- Create and switch to a new branch (optional but good practice):
```bash
git checkout -b <new-branch-name>
```
- Add and commit changes:
```bash
git add .
git commit -m "Your commit message"
```
- Push your changes to github:
```bash
git push origin <branch-name>
```

### 6. Update your local repository:

- Pull the latest changes:
```bash
git pull origin main
```

---
---

# Branches

## Branches - Basics

1. Check existing branches
```bash
git branch
```

2. Switch to the desired branch
```bash
git checkout <branch-name>
```

or

2. Create and switch to new branch
```bash
git checkout -b <new-branch-name>
```

3. Work on the branch
	(commits will be specific to that branch)

4. Push the branch to remote (if needed)
	(if a new branch and want to push it to remote repo (like github))
```bash
git push -u origin <new-branch-name>
```

---

## Deleting a branch (can be done as 2. and then 1. also)

1. Delete locally first
```bash
git branch -d <branch-name>
```

* ('-d' to ensure safety: prevents deletion if the branch is not fully merged)
* ('-D' to force delete)

2. Delete remotely after (on the remote repository)
```bash
git push origin --delete <branch-name>
```

---

## Branch Merge

1. Switch to the Main Branch:
```bash
git checkout main
```

2. Pull the latest changes:
(make sure local main branch is up to date with remote repo)
```bash
	git pull origin main
```

3. Merge the branch:
```bash
git merge <branch-name>
```
- if no confilcts, merge will complete
- else, will need to resolve them manually

4. Push the merged changes:
```bash
git push origin main
```

* (optional) Pull request:
- push the branch to github, 
- then use the github web interface to create the PR

> [!TIP] (good practice)  
> Always make sure your main branch is up to date 
> 	before merging, to reduce the likelihood of conflicts

---
---

## Basic Concept of Git Submodules:

**Submodule**: 
- A Git submodule is essentially a reference 
	to another Git repository at a particular snapshot in time.

**Independence**: 
- Changes made to the submodule are tracked in its own repository, 
	not in the parent project's repository.

**Control**: 
- You control when to update the submodule
	to newer commits from its own repository.


## Adding a submodule to a project

### (Example to add 'libft' as a submodule in a project)

1. Navigate to root directory of <project>

2. Add the submodule:
```bash
git submodule add <repository-url> <path-to-submodule>
```

* Replace <repository-url> with the URL of your libft repository.

* Replace <path-to-submodule> with the path where you want
	the submodule to reside within your project (e.g., lib/libft).

> (notice '.gitmodule' file that appeared)

3. Commit the submodule
```bash
git add .
git commit -m "Add libft as a submodule"
```

---

## Cloning a project with submodules

If we clone a project that uses a submodule, 
we need to initialize it and update the submodule

1. Clone the project
```bash
	git clone <project-repo-url>
```

2. Initialize and update submodules
	* navigate into the project directory and run:
```bash
git submodule update --init --recursive
```

---

## Working with submodules

- Pulling Changes
* (if there are updates in the 'libft' repository) update with:
```bash
	cd <path-to-submodule>
	git pull origin main
```

- commiting changes

if changes are made within the submodule, 
	commit and push from within the submodule directory, 
		and then commit the parent project as well.

---
---
