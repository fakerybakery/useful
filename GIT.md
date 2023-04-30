# Useful Git
## Ignore a file from Git history
```brew
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch debug\ log.txt' --prune-empty --tag-name-filter cat -- --all
git push --force
```
