```gnu
        .global  _start
        .data
  text: .asciz   "Welcome\n"
   len  =        .-text
        .text
_start: movq     $0x01, %rax
        movq     $1,    %rdi
        movq     $text, %rsi
        movq     $len,  %rdx
        syscall
        movq     $0x3C, %rax
        movq     $0,    %rdi
        syscall
```
