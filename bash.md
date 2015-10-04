## General

Command | Description
------- | -----------
**`#!/usr/bin/env [command]`** instead of **`#!/path/to/[command]`** | Uses the first occurance of [command] from the user's PATH
**`set -o errexit`** or **`set -e`** | exit immediately if a command exits with a non-zero status
**`set -o pipefail`** | exit if any command in a pipe fails
**`set -o nounset`** | exit when trying to use undeclared variables
**`set -x`** | print debugging information
**<code>cmd &#124;&#124; true</code>** | use this for commands that you allow to fail
**`$0`** | name of the script itself
**`$1`, `$2`, ...** | first argument, second argument etc
**`${10}`** | after 9, args must be enclosed in brackets
**`$*`** and **`$@`** | all positional parameters
**`$#`** | number of args passed
**`shift`** | reassignes potitional parameters: $1 <- $2, $2 -< $3 etc
**`if TEST-CMDS; then CMDS; fi`** | if statement
**`if TEST-CMDS; then else fi`** | if/then/else statement
**`if TEST-CMDS; then elif TEST-CMDS; elif TEST-CMDS; else fi`** | if/then/else if/else if/else
**`for NAME [in List]; do CMDS; done`** | for loop. If in list not present it uses $@
**`while CONTROL-CMD; do CMDS; done`** | while
**`ARRAY=(one two three)`** | array declaration
**`ARRAY[3]=four`** | add element
**`echo ${#ARRAY[*]}`** | print array size
**`echo ${ARRAY[*]}`** | print array
**`echo ${ARRAY[2]}`** | print element
**`delete ARRAY[1]`** | delete variable
**`unset ARRAY`** | delete array
**`FUNCTION_NAME () { CMDS; }`** | declare function
**`((a++))`** | Double parentheses for arithmetic operations
**`[[ expr ]]`** | Prefer double brackets for extended functionality (&&, ||, regexes with =~)
**`file=${1:-$DEFAULT}`** | Paremeter substitution example: provide default value for missing argument.
**`fname=$(basename "$fname")`** : Get file without path
