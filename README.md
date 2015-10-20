# git-fu
aliases and scripts to make git life better

## Git command completion for bash
https://github.com/git/git/tree/master/contrib/completion

## Git Aliases

Aliases from my `.gitconfig`:

```
[alias]
  co = checkout
  ci = commit
  st = status
  br = branch
  hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
  type = cat-file -t
  dump = cat-file -p
  fixup = !git add -A && git commit --fixup HEAD && GIT_SEQUENCE_EDITOR='echo "$REBASE_DATA"' git rebase -i HEAD~2 --autosquash
```
