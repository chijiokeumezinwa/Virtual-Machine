I was inspired to practice writing and implementing my own virtual emulator machine after reading this repository:

	https://github.com/felixangell/blog-posts/blob/main/virtual-machine-in-c.md

I did this project to get a deeper understanding of how computers work.

The source code, once compiled with Makefile, creates a Virtual Machine that is able to read a program with a sequence of instructions. 

This virtual machine is a stack based virtual machine as well as a register based virtual machine. We can push values to the stack as well as the registers.

A virtual machine follows a simple pattern, the "instruction cycle", which is: fetch; decode; and execute. First we fetch the next instruction in the instruction list or code, we then decode the instruction and execute the decoded instruction.


the listed example prog does this:
1 5; //push 5 to stack
1 1; // push 1 to stack
3; // adds 5 and 1 by popping the two values on top of the stack, and pushing the result back to stack
11 1 9 1; // if r1 == 9 branch to ip 1
0; //halt program 




