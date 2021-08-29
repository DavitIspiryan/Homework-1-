# Homework-1-

3. Can a C program be compiled or executed in the absence of a main()?

Answer:
As main function is the first function which should be written than a C program can not be executed without the main() function.

--------------------------------------------------------------------------------------------------------------------

4. Can I declare the same variable name to the variables which have different
scopes?

void function1()
{
   int variable = 0;
}
void function()
{
   int variable = 5;
}

Answer:
As they are part of different blocks of the method, we can write the same name in defferent scopes
--------------------------------------------------------------------------------------------------------------------

5. What will print the following code?

void increment(int* i)
{
    *i = *i + 1;
}
int main()
{
    int count = 7;
    increment(&count);
    printf("%d\n", count);
    return 0;
}
Answer:
I think the answer would be 8. or from 1 to 8
--------------------------------------------------------------------------------------------------------------------

6. What will print the following program?

#include <stdio.h>

int main()
{
    int x = 5641;
    if (x & 1) {
        printf("Even\n");
    } else {
        printf("Odd\n");
    }
    return 0;
}
Answer:

--------------------------------------------------------------------------------------------------------------------


7. What will print the following program, if the sizeof(int) is equal 4?

int main()
{
    int x[5];
    printf("sizeof(int)=%ld, sizeof(x)=%ld", sizeof(int), sizeof(x));
    return 0;
}

--------------------------------------------------------------------------------------------------------------------

8. What will print the following program, if as array size '7' is provided?

int main()
{
    int s = 0;
    printf("Enter array size: ");
    scanf("%d", &s);
    int* a = new int[s];
    for (int i = 0; i < s; ++i) {
        a[i] = i;
    }
    for (int i = 0; i < s; ++i) {
        printf("%d\n", a[i]);
    }
    delete [] a;
    return 0;
}

--------------------------------------------------------------------------------------------------------------------

9. What will print the following program?

struct point
{
    int x;
    int y;
};

int main()
{
    struct point p = {4, 5};
    printf("x=%d, y=%d\n", p.x, p.y);
    return 0;
}

We output x and y as integers because we are creating an example of struct point named "p" and giving values, so it will print 4, 5 as x and y
--------------------------------------------------------------------------------------------------------------------

10. Can the union elements be of different sizes?
union data
{
    char c;
    int i;
};

Answer:
No because data type can store a single variable, therefore same memory location
