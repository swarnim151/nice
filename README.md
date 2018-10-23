text:

main:

li $v0, 11        //loading the value 11 in v0 register to print a character
li $a0, 64              //PRINTING @, $a0 as @, decimal value for @ in ascii is 64
syscall

li $v0, 4        //loading the value 4 in v0 register to print an integer
addi $a0, $a0, -64       //PRINTING 0 by subtracting 64 and storing the result in $a0
syscall

addi $a0, $a0, 2      //PRINTING 2 by adding 0 and 2 and storing the result in $a0
syscall

addi $a0, $a0, 6       //PRINTING 8 by adding 2 and 6 and storing the result in $a0
syscall

addi $a0, $a0, -4      //PRINTING 4 by subtracting 4 and 8 and storing the result in $a0
syscall

addi $a0, $a0, 2       //PRINTING 6 by adding 4 and 2 and storing the result in $a0
syscall

addi $a0, $a0, -5    //PRINTING 1 by subtracting 5 from 6 and 1 and storing the result in $a0
syscall

addi $a0, $a0, 2      //PRINTING 3 by adding 1 and 2 and storing the result in $a0
sys-call

addi $a0, $a0, 6      //PRINTING 8 by adding 2 and 6 and storing the result in $a0
syscall

li $v0, 11        //loading the value 11 in v0 register to print a character
addi $a0, $a0, 2      //PRINTING newline, decimal value for [LINE FEED]in ascii is 10(8+2)
syscall




li $v0,10        //prompting the program to end
syscall
