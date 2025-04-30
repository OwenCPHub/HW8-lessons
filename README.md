# HW8-lessons

This repository covers HW#8 for CMSC 313 

there are 2 files 

HW8.asm
 this file is a simple program that prints out the message "Hello World!" this message is forst stored in the msg variable we then in the __start section declare edx with the same number of bytes needed for my message, ecx is then used to store the memory address of the message. ebx is used to store the file we want to write to. and finally eax invokes kernal opcode 4 or in other words Sys_write.

 the main issue with this file is it invokes a segmentation fault due to not having a ending

HW8lesson2.asm
  this file fixes the main issue with HW8.asm EBX is then returned to 0 meaning 0 errors and EAX calls kernal opcode 1 or SYS_EXIT. lastly it calls Int 80h to request an interupt.
