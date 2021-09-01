---
layout: default
---

# [](#header-1) 


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

* [The Limits of Quantum Computer](http://www.cs.virginia.edu/~robins/The_Limits_of_Quantum_Computers.pdf)
* [The Arithmetic of Active Management](https://web.stanford.edu/~wfsharpe/art/active/active.htm)
* [When Hubble Stared at Nothing for 100 Hours](https://www.nationalgeographic.com/science/phenomena/2015/04/24/when-hubble-stared-at-nothing-for-100-hours/)
* [1800s Astronomical Drawings vs. NASA Images](https://www.nypl.org/blog/2016/08/19/1800s-astronomical-drawings)
* [The Art of Not Taking Things Personally](https://medium.dave-bailey.com/the-art-of-not-taking-things-personally-b7a8395ce172)
