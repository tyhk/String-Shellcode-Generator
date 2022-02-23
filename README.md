# String-Shellcode-Generator
String To Little Endian Shellcode Generator

Usage: python string-to-shellcode.py \<string\>

Last step ("push esp") is to push the pointer pointing to the created string to the stack, just pop to other registry if temporary storage is nedded.
