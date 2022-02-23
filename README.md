# String-Shellcode-Generator
String To Little Endian Shellcode Generator

Usage: python string-to-shellcode.py <string>

The last step ("push esp") is to push the pointer pointing to the created string to the stack, just pop to another registry if temporary storage is needed.
