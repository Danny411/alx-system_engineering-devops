This is a folder that contains shell variables expansions, how they are used and how thry are executed


alias ls="rm *"  .....a script that creates an alias.
• Name: ls
• Value: rm * 

echo "hello $USER"  .... a script that prints hello user, where user is the current Linux user. 

PATH=$PATH:/action ..... a script that Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.


echo $(printf $PATH | tr ":" "\n" | wc -w) ..... a script that counts the number of directories in the PATH. 

printenv ..... a command that lists all environment variables 

set | less ..... a script that lists all local variables and environment variables, and functions. 

export BEST="School"  ..... a script that creates a new local variable.
• Name: BEST
• Value: School


export BEST="School"  .....  a script that creates a new global variable.
• Name: BEST
• Value: School


echo $(($TRUEKNOWLEDGE+128))  ..... a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.


echo $((POWER/DIVIDE))  .....  a script that prints the result of POWER divided by DIVIDE, followed by a new line.
• POWER and DIVIDE are environment variables


echo $(($BREATH**LOVE))  ..... a script that displays the result of BREATH to the power LOVE
• BREATH and LOVE are environment variables
• The script should display the result, followed by a new line


echo "$((2#$BINARY))"  ..... a script that converts a number from base 2 to base 10.
• The number in base 2 is stored in the environment variable BINARY
• The script should display the number in base 10, followed by a new line


echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo"  ..... a script that prints all possible combinations of two letters, except oo.
• Letters are lower cases, from a to z
• One combination per line
• The output should be alpha ordered, starting with aa
• Do not print oo
• Your script file should contain maximum 64 characters


printf "%.2f\n" $NUM ..... a script that prints a number with two decimal places, followed by a new line. The number will be stored in the environment variable NUM.


printf '%x\n' $DECIMAL  ..... a script that converts a number from base 10 to base 16.
• The number in base 10 is stored in the environment variable DECIMAL
• The script should display the number in base 16, followed by a new line


tr 'A-Za-z' 'N-ZA-Mn-za-m'  ..... a script that encodes and decodes text using the rot13 encryption. Assume ASCII. 

cat -n | grep [13579][[:space:]] | tr -s '' | cut -f2  ..... a script that prints every other line from the input, starting with the first line.



echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'bestchol')  ..... A shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result.
• WATER is in base water
• STIR is in base stir.
• The result should be in base bestchol
