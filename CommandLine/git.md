# git

## Automatically prune local branches that are no longer upstream

This one-time setting will keep your list of active branches seen via `git branch` to the actual active branches. Each time you `git pull` or `git fetch`, your local branches will be compared against their upstream branch; if the upstream branch no longer exists, the local branch is pruned.

`git config --global fetch.prune true`

## Clean up local branches that are no longer on the remote

Sometimes, the above does not work. When that happens, the following will:

To see the branches we'll remove: `git branch -vv | grep 'gone]' | awk '{print $1}'`

To delete those branches, add "| xargs git branch -D": `git branch -vv | grep 'gone]' | awk '{print $1}' | xargs git branch -D`

From Ezequiel Pérez on [Medium - Cleaning up local Git branches that no longer exist on remote](https://medium.com/@ezequiel.perez/cleaning-up-local-git-branches-that-no-longer-exist-on-remote-a038d777f8c7)