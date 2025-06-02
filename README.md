# AssemblyPlus

A programming language with modern conventions, but with the flexibility of assembly. A lot of programming languages take after C, but C was made to be a portable assembly. Other languages aim to simplify the development process to allow for the human mind to worry about the problem and not the registers. 

AssemblyPlus takes a different approach. Instead of taking after C, take after assembly. The language is a virtual machine, that matches closely with modern hardware. An example is shown below

```
// Fibonaci
func fib(u32 n)
START
MOV R0, 0
MOV R1, 1
MOV R2, 0
MOV R3, n
Loop_Begin
ADD R2, R1, R0
MOV R1, R0
MOV R2, R1
DEC R3
LOOP R3 > 0 to Loop_Begin
Loop_End
PUSH 
END
```
