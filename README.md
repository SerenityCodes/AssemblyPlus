# AssemblyPlus

A programming language with modern conventions, but with the flexibility of assembly. A lot of programming languages take after C, but C was made to be a portable assembly. Other languages aim to simplify the development process to allow for the human mind to worry about the problem and not the registers. 

AssemblyPlus takes a different approach. Instead of taking after C, take after assembly. The language is a virtual machine, that matches closely with modern hardware. An example is shown below

```
// Fibonaci
func fib(u32 n)
START
R0 = 0;
R1 = 1;
R2 = 0;
R3 = n;
Loop_Begin
R2 = R0 + R1;
R0 = R1; 
R1 = R2;
R3--;
LOOP R3 > 0 to Loop_Begin
Loop_End
PUSH R2
END
```
