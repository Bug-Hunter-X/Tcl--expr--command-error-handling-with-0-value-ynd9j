# Tcl 'expr' command error handling with 0 value

This repository contains a Tcl script demonstrating a potential issue with the 'expr' command's handling of the value 0. When the script attempts to use 0 in an arithmetic expression within 'expr', it will produce an error. The provided solution fixes the error by checking for the value 0 using a simple 'if' statement before calling the 'expr' command.

## Bug Description
The bug is caused by the unexpected behavior of Tcl's 'expr' command when encountering a value of 0 in an arithmetic operation. A simple check for 0 before the 'expr' command resolves this issue. This repository illustrates the bug and its solution using a simple Tcl procedure.

## How to Reproduce
1. Clone the repository.
2. Run the script using a Tcl interpreter. 

The script should produce an error because the 'expr' command cannot handle 0 properly. 

## Solution
The solution involves adding a simple check for 0 before calling the 'expr' command. If the input is 0, the function returns 0 directly, avoiding the problem with the 'expr' command.