# c-functions 🎀
```c
#include <stdio.h>

void line();
// no arg no return (4)
void greetings();

// with arg no return (3)
void checker (int up, int upp);

// no arg with return (2)
int fixed ();

// with arg and return (1)
int calcu (int num, int nums);

int main () {
	
	// (4)
	greetings();
	line ();
	
	// (3)
	int up;
	int upp;
	checker (0, 0);
	line ();
	
	// (2)
	int f = fixed();
	if (f <= 5) {
		printf("CORRECT!! Fixed value is %d\n", f);
	} else {
		printf("WRONG FIXED VALUE!\n");
	}
	
	// (1)
	line();
	int num;
	int nums;
	printf("\nInput two numbers to add: ");
	scanf("%d %d", &num, &nums);
	calcu (num, nums);
	
	
	
	return 0;
}

void line () {
	printf("--------------------------------------------------");
}

// (4)
void greetings () {
	printf("WELCOME NOOBS! THIS IS A MINI CACLU!!!\n");
}

// (3)
void checker (int up, int upp) {
	printf("\nPut two numbers: ");
	scanf("%d %d", &up , &upp); 
	if (up % 2 == 0) {
		printf("The first number is EVEN!\n");
	} else {
		printf("The first number is ODD!\n");
	}
}

// (2)
int fixed () {
	int value;
	printf("\nFixed value is a number that is below 5: ");
	scanf("%d", &value);
	return value;
}

// (1)
int calcu (int num, int nums) {
	
	int combi;
	combi = num + nums;
	printf("The sum of %d and %d is %d", num, nums, combi);
	
	
	return combi;
}
```
