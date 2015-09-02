## Git Internals

Command | Description
------- | -----------
**`git hash-object [file]`** | Find the SHA-1 hash of [file] that will be stored in .git/objects
**`git hash-object --stdin`** | Same as above, with extra option to read content from stdin
**`git cat-file -p [hash key]`** | See the contents of the object with [hash key]
**`git cat-file -t [hash key]`** | See type of object with [hash ley]
**`git ls-files -s`** | Show index with file mode and hash of every file.

## Git Undoing

Command | Description
------- | -----------
**`git revert [SHA]`** | Create a new commit that is the inverse of the given SHA. Does not alter history. So you can git push.
**`git commit --amend`** | Edit message/files and update most recent commit (before git push)
**`git checkout -- [file/dir]`** | Undo local changes. Alters file/dir by checking out HEAD, the last commit. Working dir changes are forever lost.
**`git reset [last good SHA]`** | Undo commits by rewinding to specified SHA. Add --hard to undo both commits and working dir changes.
**`git reflog`** | Bring git-reset --hard changes back to life. Works for limited time (git garbage collection)
**`git branch f; git reset --hard origin/master; git co f`** | Tranfer commits from master to f
**`git rebase -i HEAD~3`** | Rearrange/edit last 3 commits


## Git History Viewing

Command | Description
------- | -----------
**`git log -2`** | Show 2 last commits
**`git log --stat`** | Show statistics of files modified
**`git log -S`** | Only show commits adding or removing code matching the string
**`git cat-file -p [commit SHA]`** | Pretty-print the contents of commit. Useful for finding commiter/author.

## Git Remote Management

Command | Description
------- | -----------
**`git reset --hard <commit-hash>`** & **` git push -f origin master`** | Revert remote commit. Use with caution.


## Git Misc Tips

Command | Description
------- | -----------
**`git merge --no-ff`** | Construct a merge instead of fast-forwarding, to ensure that merges are explicitly shown in history.
