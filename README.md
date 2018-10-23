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

addi $a0, $a0, 56      //PRINTING 'B', decimal value for 'B' in ascii is 66(10+56)
syscall

addi $a0, $a0, 38     //PRINTING 'h', decimal value for 'h' in ascii is 104(66+38)
syscall

addi $a0, $a0, -7      //PRINTING 'a', decimal value for 'a' in ascii is 97(104-7)
syscall

addi $a0, $a0, 13      //PRINTING 'n', decimal value for 'n' in ascii is 110(97+13)
syscall

addi $a0, $a0, -10      //PRINTING 'd', decimal value for 'd' in ascii is 100(110-10)
syscall

addi $a0, $a0, -3      //PRINTING 'a', decimal value for 'a' in ascii is 97(100-3)
syscall

addi $a0, $a0, 17      //PRINTING 'r', decimal value for 'r' in ascii is 114(97+17)
syscall

addi $a0, $a0, -9      //PRINTING 'i', decimal value for 'i' in ascii is 105(114-9)
syscall





li $v0,10        //prompting the program to end
syscall
