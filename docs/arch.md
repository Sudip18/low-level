# Architecture

In order to run some software you need a real machine and
real machines come with a great variety of architecture

 - [Function calls in C: the boring specs](http://www.gghh.name/dibtp/2015/11/10/function-calls-in-c-the-boring-specs.html)
 - [Function calls in C: a practical example](http://www.gghh.name/dibtp/2015/11/11/function-calls-in-c-practical-example.html)

## Assembler

There are two notations: **Intel** and **AT&T**.

 - [Intel and AT&T Syntax](http://www.imada.sdu.dk/Courses/DM18/Litteratur/IntelnATT.htm)
 - [GNU As manual](http://tigcc.ticalc.org/doc/gnuasm.html)

## X86

 - [Assembly Wikibook](https://en.wikibooks.org/wiki/X86_Assembly)
 - [A fundamental introduction to x86 assembly programming](https://www.nayuki.io/page/a-fundamental-introduction-to-x86-assembly-programming)
 - [The mysteries arround "0x7C00" in x86 architecture bios bootloader](http://www.glamenv-septzen.net/en/view/6)
 - [Shellcode obfuscation](https://breakdev.org/x86-shellcode-obfuscation-part-2/) talk about internal format of opcode

## AMD64

1. User-level applications use as integer registers for passing the sequence %rdi, %rsi, %rdx, %rcx, %r8 and %r9. The kernel interface uses %rdi, %rsi, %rdx, %r10, %r8 and %r9.
2. A system-call is done via the syscall instruction. The kernel destroys registers %rcx and %r11.
3. The number of the syscall has to be passed in register %rax.
4. System-calls are limited to six arguments, no argument is passed directly on the stack.
5. Returning from the syscall, register %rax contains the result of the system-call. A value in the range between -4095 and -1 indicates an error, it is -errno.
6. Only values of class INTEGER or class MEMORY are passed to the kernel.

 - [Gentle Introduction to x86-64 Assembly](http://www.x86-64.org/documentation/assembly.html)

## ARM

 - [Reverse engineering the ARM1](http://www.righto.com/2015/12/reverse-engineering-arm1-ancestor-of.html)
 - [More ARM1 processor reverse engineering: the priority encoder](http://www.righto.com/2016/01/more-arm1-processor-reverse-engineering.html)

## SPARC

## RISC

## POWERPC

## Links

 - What every programmer should know about memory, Part 1 [LWN](http://lwn.net/Articles/250967/)
 - [Baking Pi – Operating Systems Development](https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/os/)
