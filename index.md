---
layout: default
---

# [](#header-1) Site Under Construction


```nasm
; Nasm. Linux x64

        global  _start

        section .text
_start:
        ; write(1, message, 13
        mov     rax, 1                 
        mov     rdi, 1                 
        mov     rsi, message          
        mov     rdx, 13               
        syscall                       

        ; exit(0)
        mov     eax, 60               
        xor     rdi, rdi              
        syscall                       
message:
        db      "Hello, World", 10    

```
## [](#header-2)Interesting Reads

*   [The Limits of Quantum Computer](http://www.cs.virginia.edu/~robins/The_Limits_of_Quantum_Computers.pdf).
