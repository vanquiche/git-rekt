# Getting Started

Before any staging, commits, branching, etc you must initialize git into your working repository. To do that simply use the command:

  > git init

Once git is initialize, any file and thier changes will be tracked by git. If there are files or folders that you would like git to ignore, simply create an

  > .gitignore

and list files/folders to omit. Anything listed inside the .gitignore file will not be tracked, nor will it be pushed to a remote repository i.e. GitHub.

# Staging

Git will notice any new files and lines of code that you create but they will not be tracked until they're staged. To stage a file use the command

  > git add <filename>
  > or to stage all files use the command:
  > git add .
  >
  > to see what is staged or untracked use the command:
  > git status

Once a file is staged, git will track any modifications you make. Mind you these new changes will not be in the staging area for commit. You'll have to stage those new changes if you plan to include it into the next commit. To view the changes you can use the command:

  > git diff <filename>

# Commit

You can think of commits as a snapshot that you can return to. Once you feel like you've reached a good spot in development to create a snapshot, stage the appropriate files (git add) then use the command:

  > git commit
  > the default editor will open for you to write a commit message
  > or use the shorthand command:
  > git commit -m 'your commit message'
  >
  > to view a list of your commits use the command:
  > git log

  > to change the default editor to your choice, use the command:
  > git config --global core.editor"<editor>"

One of the core features of git is the ability to jump to previous moments in the development history. For this to be effective, it's key to ensure your commits (snapshots) are small with specific messages.

When writing a commit message think of the "why?" and "what?".

# Branches

In the beginning of development our default branch is the "main" branch. Working on this branch exclusively is fine in the early stages of development but as its complexity grows we want to create new branches often when working on additional features. This allows for others to work in tandem or experimentation while preserving our base code.
To create a new branch use the commmand:

  > git branch <branch-name>
  >
  > to switch branches use the command:
  > git checkout <branch-name>
  >
  > or use the shorthand:
  >
  > git checkout -b <branch-name>
  > to create a branch and checkout all at once
  >
  > to view all branches use the command:
  > git branch

# Next Stop

If you made it to this point, use the 'git branch' command to view all branches.'checkout' a branch to get more details on a specific subject. Cheers!