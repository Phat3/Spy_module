Spy_module
==========

A simple module that tricks system call handler

this module operate in this manner:

1. A User-space process call the sys_open

2. The sys_open number is passed to the kernel

3. The system_call() function check the number

4. Go to the right cell of the table

5. Execute the function in the row, that is not sys_open but our_sys_open (explain n the code how to do this)

6. The return value of our_sys_open is the execution of the right syscall sys_open
