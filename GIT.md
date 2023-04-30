# Useful Git
## Delete a file from all previous Git commits (works on GitHub)
```brew
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch debug\ log.txt' --prune-empty --tag-name-filter cat -- --all
git push --force
```
