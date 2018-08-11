# Hello-Word
Hello Word no iostream functions call

code is

<pre>
__asm {
    mov edi, [esp + 4]
    sub edi, 0x200
    mov eax, edi
    add eax, 0x100
    push eax
    call [edi]
    mov eax, edi
    add eax, 0x110
    push eax
    call [edi + 4]
    add esp, 8
    ret
 }
</pre>
