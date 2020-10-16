```asm
        [bits    64]
        section  .data
  text: db       "hello, world!", 0hA
   len: equ      $-text
        section  .text
        global   _start
_start: mov      rax, 0h01
        mov      rdi, 1
        mov      rsi, text
        mov      rdx, len
        syscall
        mov      rax, 0h3C
        xor      rdi, rdi
        syscall
```
