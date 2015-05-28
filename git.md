Command | Description
------- | -----------


## Git internals

Command | Description
------- | -----------
git hash-object [file] | Find the SHA-1 hash of [file] that will be stored in .git/objects
git hash-object --stdin | Same as above, with extra option to read content from stdin
git cat-file -p [hash key] | See the contents of the object with [hash key]
git cat-file -t [hash key] | See type of object with [hash ley]
