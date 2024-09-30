# Local
- working tree
- index
- local branch
- remote-tracking branch
    - copy of remote repo


# Fetch
- git fetch
    - download the copy of remote repo
        - i.e. update the remote-tracking branch.
    - it doesn't affect to the working tree

- we can watch remote-tracking branch by
    - origin/\<branch-name\>
- we can merge to local by
    - git merge origin/\<branch-name\>

# Merge
- fast-forward 
    - integrate the histories to the current tip
- non-fast-forward
    - fast-forward \& Make the merge commit in git log.

- In one word, apply the commits(develop) on the current(main) branch.


# Rebase
- Save the commits and reset --hard
- Acoomplish the commits by creating new commits and apply on the branch.

- In one word, create the commits(develop) on the current(main) branch on the tip.


# Pull or Pull --rebase
- git pull
    - git fetch origin/\<branch-name\>
    - git merge origin/\<branch-name\>
    - with merge commit.
- git pull --rebase
    - git fetch origin/\<branch-name\>
    - git rebase origin/\<branch-name\>
    - without merge commit!!!