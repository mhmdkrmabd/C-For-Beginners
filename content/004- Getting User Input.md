In order to get user input, regards the type of that input, we can use `scanf()`.

An example of getting integer input from the user:

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    // Get age from the user
    int age;
    printf("Enter your age: ");
    // & = Pointer, must be used with most of the date types
    scanf("%d", &age);
    printf("You're %d years old.\n", age);

    return 0;
}
```

Example of getting double from the user

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    // Get GPA from the user
    double gpa;
    printf("Enter your GPA: ");
    // %lf is used for scanf, it can also be used with printf alongside %f
    scanf("%lf", &gpa);
    printf("Your GPA is %lf.\n", gpa);
    return 0;
}
```

Example of getting character from the user:

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    // Get grade from the user
    char grade;
    printf("Enter your grade: ");
    scanf("%c", &grade);
    printf("Your grade is %c.\n", grade);

    return 0;
}
```

Final example of getting a string from the user:

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    // Get name from the user
    char name[20];
    printf("Enter your name: ");
    // By using scanf, we won't be able to get the input after whitespace
    // scanf("%s", name);
    // So, we need to use fgets()
    fgets(name, 20, stdin);
    printf("Your name is %s.\n", name);

    return 0;
}
```
