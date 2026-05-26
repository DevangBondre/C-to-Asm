#Objective 
C code which prints the sum of all elements of an array

#Tools used 
Visual studio : Used to write C code and compile it into an executable.
Ghidra : Static analysis 
X64Dbg : Dynamic analysis

#Exe build 
This program was compiled in debug build with 0d optimization.

#Source code

![source code](images/source%20code.PNG)

The code logic is very simple it has a array of integers which is getting passed through a loop in a 
function called "sum_array". Where the value of sum is initially set to 0 and this value gets updated 
as the loop runs resulting in addition of every element into the sum wtih each loop and the function then 
returns the final value of sum  which is then used in the printf statement.

![decompiled C](images/decompiled%20C.PNG)

After you build the C program and analyze it in Ghidra you can find the main function using the Strings feature where 
you can find the "The sum of array is" string which is hardcoded in the original C code.

Inside the main function we can see 