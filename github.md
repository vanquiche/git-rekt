# GitHub

To get a local copy of a remote repository (whether it be yours, a forked repo, or another owners) you can use the clone command as such:

  > git clone 'path-to-repo'
  >
  > the path can either be via SHH or HTTPS link

With a local copy of the repository you can add files, make changes, and event make commits.

To upload those changes back to the remote repository use the push command:

  > git push origin 'branch'
  >
  > note: unless you are a member of a repository you will only have permission to push to your own repositories (including forked repos).

If you're working on a shared repository and want to aquire the most recent working copy use the pull command:

  > git pull
  >
  > the pull command will fetch and merge to the most recent update.
  >
  > if you want the latest update without a merge use:
  >
  > git fetch

# What is 'origin'

origin represents the repository path that our current working tree points to. This is where we are pushing and pulling from. To view this use the command:

  > git remote -v



