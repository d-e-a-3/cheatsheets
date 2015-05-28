Command | Description
------- | ----------
h,j,k,l | left, down, up, right - Considered more efficient than using the arrow keys
:noh | Disable highlighting (After search)
/ | Search
? | Backwards search
o / O | Insert new line after/before the current one
A | Go to the end of line and append
b | Go back a word
db | Delete preceding word
w | Go forward a word
dw | Delete next word
cw | Change next word
yy | Copy line
p | Paste line
0 | Go to the starting of current line
^ | Go to the first non blank character of the line.
$ | Go to the end of the current line.
G | Go to the end of the file.
nG / :n | Move to n'th line of file
{ / } | Go to the beginning/end of the current paragraph
% | Go to the matching braces or parenthesis inside code
C-f / C-b | scroll screen forward / backward
C-g | Show status
z. | Put the line with the cursor at the center
zt | Put the line with the cursor at the top
zb | Put the line with the cursor at the bottom of the screen
s | Substitute character
d$ | Delete to the end of the line.
:s/old/new | To substitute new for the first old in a line type
:s/old/new/g | To substitute new for all 'old's on a line type
:#,#s/old/new/g | To substitute phrases between two line #'s type
:%s/old/new/g | To substitute all occurrences in the file type
:%s/old/new/gc | To ask for confirmation each time add 'c'
:r FILENAME | Insert the contents of a file
:r !ls | Read the output of the command and insert it below the cursor
v  motion  :w FILENAME | saves the Visually selected lines in file FILENAME
:setlocal spell spelllang=en_us | Enable spellcheck
zg | Add the word that is under the cursor into (~/.vim/spell/spellfile
:sp | Split windows horizontally
:vsp | Split windows vertically
