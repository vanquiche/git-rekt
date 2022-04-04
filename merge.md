# Merge

Eventually we will want to intergrate our code back into a single branch. The merge command is the most commonly used way to combine two branches. When this operation is performed the selected (checked out) branch will be updated to reflect the merge, while the target branch will be unaffected.

To merge your branches:

  > checkout the branch you want to update
  >
  > git checkout 'branch'
  >
  > git merge 'target-branch'
  >
  > if you'd like to delete a branch, use the command:
  >
  > git branch -d 'branch'

There is another utility to combine branches called "rebase" that I will cover in separate module. It can be intimidating because rebase will reshape the tree to appear in a linear path in contrast to the parallel paths of "merge". What this means is that it will rewrite history by replacing a previous commit with a new one.

