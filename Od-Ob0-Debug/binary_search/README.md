## Objective

C code which takes a number as a user input and searches the number in the existing array using binary search and prints out the `index at which number was found` or print `not found` if the number is not present in the array.


## Tools used

**Visual studio** : Used to write C code and compile it into an executable.<br>
**Ghidra** : Static analysis <br>
**X64Dbg** : Dynamic analysis<br>


## Exe build:

This program was compiled in `debug build` with `0d` optimization and `default inline function expansion` <br>


# Source code

```c 

#include <stdio.h>

int main(void) {
	int user_input;
	printf("What is the number you want to search : ");
	scanf_s("%d", &user_input);
	int array[] = {1,5,7,11,19};
	int size = sizeof(array) / sizeof(array[0]);
	int left = 0;
	int right = size - 1;
	
	while (left <= right) {
		int mid = (left + right) / 2;
		if (user_input == array[mid]) {
			printf("Found %d at index %d", user_input,mid);
			return 0;
		}
		else if (user_input > array[mid]) {
			left = mid + 1;
		}
		else {
			right = mid - 1;
		}
	}
	printf("Number not found");
}

```


