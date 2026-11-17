# Using `git ub`

`git ub` is not a built-in Git command. If you mean “update my current branch from its upstream,” define an alias:

```sh
git config --global alias.ub '!git fetch && git rebase @{u}'
```

Then, on a branch with an upstream configured, run:

```sh
git ub
```

This fetches remote changes and rebases your current branch onto its upstream. Check the upstream with `git branch -vv`; set one with `git push -u origin <branch>`. If `ub` is already defined in your setup, inspect it with `git config --get alias.ub`.


# THIS IS MAIN MAIN BRANCH
# this is 2.0