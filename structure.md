### View content of the staging area
`git ls-files -s`

### Stage interactively
`git add -p`

### Undo the staging of your file
`git reset`

### Create a tag (simply a pointer to a commit)
`git tag <tag_name>`

### List the tags
`git tag`

### View the content of a tag
`git show <tag_name>`

### Create an annotated tag: A tag that stores additional info
`git tag -a <tag_name> -m '<additoonal info>'`

### List all tags and the commit they point to
`git show-ref --tags`

### List all tags pointing at a commit
`git tag --points-at <commit_id>`

### Look at your other refs to HEAD in a repository
`git show-ref heads`

### View your log in your terminal as opposed to opening on a new screen
`git --no-pager log`

### Print logs on one line each
`git log --oneline`

### To force a merge commit when merging (no fast-forwarding)
`git merge <feature_branch> --no-ff`

