To check untracked files that Git LFS should track, use:

```
git status --short
```

Then list untracked files only:

```
git ls-files --others --exclude-standard
```

### Check which untracked files match Git LFS patterns

```
git lfs track
```

This shows configured LFS tracking patterns in `.gitattributes`.

To find untracked files matching LFS rules:

```
git ls-files --others --exclude-standard |
while read -r file; do
    git check-attr filter -- "$file" | grep -q 'filter: lfs' && echo "$file"
done
```

### Check files that should be tracked by LFS but aren't

```
git lfs migrate info --everything
```

This reports files that could be migrated to LFS based on size and history.

Important: Git LFS doesn't automatically track untracked files. You must add them:

```
git add path/to/file
```

If the file matches an LFS pattern, Git will store it through LFS when committed.

