<img align="right" width="50%" alt="top langs" src="https://github-readme-stats.vercel.app/api/top-langs/?username=llathasa-veleth">

```asm
        [bits    64]
        section  .data
  text: db       "welcome!", 0hA
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
