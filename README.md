# comporg_simulation1

Computer Organization - Spring 2024
==============================================================
## Iran Univeristy of Science and Technology
## Assignment 1: Assembly code execution on phoeniX RISC-V core

- Name:pouria masoumi
- Team Members:ashkan ghasemineghad
- Student ID: 400414084





name: ashkan ghaseminezhad team member: pooria masoomi student id : 400414093

report
for square root code the steps are :

Load n (144) into register x4. Initialize lo (low bound) to 0 in register x5. initialize hi (high bound) to n (144) in register x6.

Compute the midpoint mid as (lo+hi)/2 (lo+hi)/2 and store it in x7. Calculate mid^2 and store it in x8. Check if mid^2 is equal to n. If so, jump to done. If mid^2 is less than n, adjust lo to mid + 1 and jump back to the start of the loop. If mid^2 is greater than n, adjust hi to mid - 1 and check if the loop should continue.

The ebreak instruction is used to exit the program, which may need to be replaced by an actual exit system call depending on the execution environment.

report 2
The function saves the necessary registers on the stack. The base address of the array and indices are stored in s0, s1, and s2. If end is less than start, the function returns. The PARTITION function is called to get the pivot index. QuickSort is recursively called for the subarrays before and after the pivot. The saved registers are restored, and the function returns.

The function saves the return address on the stack. The pivot element is set to the last element of the current subarray. The main loop iterates over the subarray, swapping elements as needed to partition around the pivot. After the loop, the pivot is placed in its correct position. The new pivot index (i + 1) is returned.

EXIT: ebreak # Exit the program The program exits by triggering a breakpoint
