ARM cross compiler Cross-compilation is the process of compiling code
for one computer system (also known as the target) on a different system,
called the host. A cross compiler is a type of compiler, that generates machine
code targeted to run on a system different than the one genrating it.Like we
used arm cross compiler to convert from X86 processsor to ARM. The Process
of creating executable code for different machines is called retargeting.The
cross compiler is also called as retargetable compiler.We have usesd GNU
GCC cross compiler. A cross compiler is a compiler capable of creating
executable code for a platform other than the one on which the compiler is
running. For example, a compiler that runs on a X86 processor but generates
code that runs on ARM Processor is a cross compiler.


1.Visit the link :https : //www.acmesystems.it/arm9toolchain
2.As I am using an Arietta, open the terminal of ubuntu(by crtl+alt+t)
write:
sudoapt−getinstallgcc−arm−linux−gnueabig++−arm−linux−gnueabi
3.After writing the above code, package will start downloading.
4.You are ready to use ARM cross compile


Program Tracing

For each line of the program, explaining each line of assembly code.
1.The push instruction at the beginning of this function: Pushes the return
address, the value contained in the lr register, onto the stack,the value contained in the fp register, onto the stack. Updates the sp to show that two
32-bit values have been pushed onto the top of the stack.
2.This instruction doesn’t set fp to 4, but rather to the current value of
sp. fp serves as a reference to local information on the stack that remains
constant during the execution of F. The old frame pointer, parameters and
local variables are then stored at negative offsets from fp. 3.The parameters
are passed in Registers r0 (a) and r1 (b); this is a convention defined in the
Procedure Call Standard for the ARM Architecture.
3.Here, 8 Bytes of space are reserved on the stack, so that subsequent stack
operations do not modify the local stack frame.
4.This copies r0 (Parameter a) into the local stack frame at address fp-8.
5.Loads r0 with .L3 contents
6.print string and pass parameters into r0, r1, and r2
7. Moves the constant value 0 in r0.
8.moves the value from r3 to r0.
9.pop the value out of pc
