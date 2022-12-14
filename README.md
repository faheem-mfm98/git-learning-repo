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
git add <filename_or_full_path_to_file>
```

Above commmand adds a modified file to the staging so it may be committed later.
**Note:** You cannot add an empty folder to vcs using git. Folders that consist at least one file
can be added by adding the file(s) that is inside the folder. 

For example, the sample folder with sample_file2 is created by running  the following command:

```
git add sample_folder/sample_file2 // full path to file is given 
```

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
You can check whether you have rights to push or not, run:

```
git remote -v

// the command gives the output as: remote_repo_shortname url_to_it privilege

origin url_to_repo (fetch)
origin url_to_repo (push)
```

**fetch**: you can fetch the files from the repo.
**push**: you can push commits to the repo.

If you don't see the push, then you don't have the privilege to make changes to the repo.

### Configuring User for Rights

Git requires user email to for audit changes to repositories. 

```
git config user.email "example@example.com"
```

Now, you should be able to push changes to the repository.
