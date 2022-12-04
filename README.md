# git-learning-repo
This repo is made for learning and documenting my git learning journey. 


## Git Commands

### Convert a local Directory into a Git Repository

To make a directory (folder) that is on your machine available on version control system such github, first open the directory in the terminal and then run:

```
git init
```

Your directory will be tracked by git and will be version-controlled by git.

### Getting A Local Access to a Repository

To get a copy of a repo on your machine, clone it using:

```
git clone <url_of_this_repo>
```

The url is available in the **Code** drop-down menu above.

### Staging Changes / Modifications

Staging means to store changes that are made in a file or directory for the purpose of putting all changes in one place.

```
git add <filename_or_path>
```

Above commmand adds a modified file to the staging so it may be committed later.

### Commiting a Stagged environment

The stagged files are commited to create a permanant change to the files or directory.
This is the new version of the directory. 

```
git commit <flags>
```

Above command commits and creates a new version of the directory based on modifications available in staging environment.

### Pushing Commits to Remote Repository

To push is to make the commits appear on a remote repository over a network.

```
git push <remote_repo_name> <branch_name>
```

Git assigns the shortname **origin** to cloned remote repositories. Branch name could **main**.

### Configuring User for Rights

Git requires user email to for audit changes to repositories. 

```
git config user.email "example@example.com"
```

Now, you should be able to push changes to the repository.
