### Movement

Command | Description
------- | ----------
h,j,k,l | left, down, up, right - Considered more efficient than using the arrow keys
b | Go back a word
w | Go forward a word
0 | Go to the starting of current line
^ | Go to the first non blank character of the line.
$ | Go to the end of the current line.
G | Go to the end of the file.
nG / :n | Move to n-th line of file
{ / } | Go to the beginning/end of the current paragraph
% | Go to the matching braces or parenthesis inside code
C-f / C-b | scroll screen forward / backward
C-d / C-u | Go down/up
Ctrl-o | Go to previous cursor location

### Edit

Command | Description
------- | ----------
db | Delete preceding word
dw | Delete next word
d$ | Delete to the end of the line.
cw | Change next word
ci<char> | Change inside <char> e.g. ci( to change inside parenthesis
s | Substitute character
o / O | Insert new line after/before the current one
A | Go to the end of line and append
yy | Copy line
p | Paste line

### Search

Command | Description
------- | ----------
/ | Search
? | Backwards search
:noh | Disable highlighting (After search)
:s/old/new | To substitute new for the first old in a line
:s/old/new/g | To substitute new for all 'old's on a line
:#,#s/old/new/g | To substitute phrases between two lines
:%s/old/new/g | To substitute all occurrences in the file type
:%s/old/new/gc | To ask for confirmation each time add 'c'

### Ctags

Command | Description
------- | ----------
Ctrl-] | Jump to the tag underneath the cursor
:ts <tag> <RET> | Search for a particular tag
:tn | Go to the next definition for the last tag
:tp | Go to the previous definition for the last tag
:ts | List all of the definitions of the last tag
Ctrl-t | Jump back up in the tag stack

### Misc

Command | Description
------- | ----------
C-g | Show status
z. | Put the line with the cursor at the center
zt | Put the line with the cursor at the top
zb | Put the line with the cursor at the bottom of the screen
:r FILENAME | Insert the contents of a file
:r !ls | Read the output of the command and insert it below the cursor
v motion :w FILENAME | saves the Visually selected lines in file FILENAME
:setlocal spell spelllang=en_us | Enable spellcheck
zg | Add the word that is under the cursor into (~/.vim/spell/spellfile
:sp | Split windows horizontally
:vsp | Split windows vertically
