# String-Shellcode-Generator
String To Little Endian Shellcode Generator

Usage: python stringtoshell.py <STRING>

Example 1. (9 chars)
C:\> python stringtoshell.py ntdll.dll
xor   eax, eax
mov   al, 0x6c
push  eax
push  0x6c642e6c
push  0x6c64746e

Example 2. (10 chars)
C:\> python stringtoshell.py nvcuda.dll
xor   eax, eax
mov   ax, 0x6c6c
push  eax
push  0x642e6164
push  0x7563766e

Example 3. (11 chars)
C:\> python stringtoshell.py shell32.dll
xor   eax, eax
mov   al, 0x6c
shl   eax, 0x10
add   ax, 0x6c64
push  eax
push  0x2e32336c
push  0x6c656873
  
Example 4.
C:\> python stringtoshell.py https://www.google.com
xor   eax, eax
mov   ax, 0x6d6f
push  eax
push  0x632e656c
push  0x676f6f67
push  0x2e777777
push  0x2f2f3a73
push  0x70747468
