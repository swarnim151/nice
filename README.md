text:

main:

li $v0, 11        //loading the value 11 in v0 register to print a character
li $a0, 64              //PRINTING @, $a0 as @, decimal value for @ in ascii is 64
syscall





li $v0,10        //prompting the program to end
syscall
