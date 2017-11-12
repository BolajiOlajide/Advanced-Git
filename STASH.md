### Keep untracked files
`git stash --include-untracked`

### Keep all files (even the ignored ones)
`git stash --all`

### Apply a specific stash
`git stash apply stash@{stash-number}

### Print the type of data stored in a SHA1
`git cat-file 8fadb -t`

### Print the data stored in a SHA1
`git cat-file 8fadb -p`

### Name stashes for easy references
`git stash save 'WIP: Progress with ...'`

### Start a new branch from a stash
`git stash branch <branch_name>`

### Grab a single file from a stash
`git checkout <stash name> -- <filename>

### Remove the last stash and apply the changes
`git stash pop` - doesn't remove if there's a merge conflict

### Remove the last stash
`git stash drop`

### Remove the nth stash
`git stash drop stash@{n}`

### remove all stashes
`git stash clear`

### To peek into a stash
`git stash show <stash reference>

### List all stashes
`git stash list`

### Add specific parts of a file to your staging area
`git add -p`

### Stash specific parts of a file
`git stash -p`
