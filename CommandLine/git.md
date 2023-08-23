# git

## Automatically prune local branches that are no longer upstream

This one-time setting will keep your list of active branches seen via `git branch` to the actual active branches. Each time you `git pull` or `git fetch`, your local branches will be compared against their upstream branche; if the upstream branch no longer exists, the local branch is pruned.

`git config --global fetch.prune true`
