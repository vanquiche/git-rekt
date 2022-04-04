# Stash

the stash command is perfect if you've been writing some code and suddenly need to revert to the original state, but you would like to keep the changes you've made. I like to think of the stash command as a "cut" and "paste" operation.

to stash local changes use the command:

  > git stash
  > or to attach a message
  > git stash save <'write a message'>

This will stash your changes into an index list.
to view a list of current stash entries use the command:

  > git stash list

to "paste" a stash entry back into your working directory you a few options:

  > git stash apply <index>
  > will apply the stash, while preserving the entry in the list

  > git stash pop <index>
  > will apply the stash and remove the entry from the list

to clean up your stash list use the command:

  > git stash drop <index>
  > will remove the specified entry from list

  > git stash clear
  > will remove all entries

Something to keep in mind is that is saved locally so it's not something you could push or pull remotely.

# Use Case

The most common use of stash would be in a scenario where you need to switch branches before you're ready to make a commit on the current branch. Stashing will remove your changes from the working tree, thus allowing you to switch branches.

Once you return to the original branch you may apply or pop your stashed changes and pick up where you left off.