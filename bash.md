Command | Description
------- | -----------
Using #!/usr/bin/env [command] instead of #!/path/to/[command] | Uses the first occurance of [command] from the user's PATH
set -e (or set -o errexit)|  Exit immediately if a command exits with a non-zero status.
$0 | name of the script itself
$1 $2 | first argument, second argument etc
${10} | after 9, args must be enclosed in brackets
$* and $@ | all positional parameters
$# | number of args passed
shift | reassignes potitional parameters: $1 <- $2, $2 -< $3 etc
if [ TEST-CMD ]; then CMDS; fi | if
if-then-else-fi | if - then - else
if-then-elif-elif-else-fi | if - then - else if - else if - else
for NAME [in List]; do CMDS; done | for loop. If in list not present use $@
while CONTROL-CMD; do CMDS; done | while
ARRAY=(one two three) | array declare
ARRAY[3]=four | add element
echo ${#ARRAY[*]} | print array size
echo ${ARRAY[*]} | print array
echo ${ARRAY[2]} | print element
delete ARRAY[1] | delete variable
unset ARRAY | delete array
FUNCTION_NAME () { CMDS; } | declare function

