> Variable is a container that stores data.

The following block of code shows how to define and use two variables in C.

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    // Without [] we'll be able to store only one character.
    char name[] = "Tom";
    int age = 80;
    // By using %s we're telling printf that we want to print string variable
    printf("There once was a man named %s\n", name);
    printf("he was %d years old.\n", age);
    printf("He really liked the name %s.\n", name);
    printf("but didn't like being %d.\n", age);
    return 0;
}
```

In C, there are many types of data that cen be defined:

| Data Type        | C Definition | Print Percentage Abbr | Example        |
| ---------------- | ------------ | --------------------- | -------------- |
| Numbers: Integer | `int`        | `%d`                  | 1, 15, 20      |
| Numbers: Double  | `double`     | `%f`                  | 5.2, 3.14, 8.9 |
| Numbers: Float   | `float`      | `%f`                  | Like double    |
| Text: Charachter | `char`       | `%c`                  | 'A'            |
| Text: String     | `char`       | `%s`                  | "Mohammaed"    |

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
  // Make the variable constant
  const int   num_integer       = 22;
  double      num_double        = 12.0;
  float       num_float         = 1997.0;
  char    txt_charachter    = 'A';
  char    txt_word[]        = "Mohammaed";

  printf("Print Integer %d.\n"  , num_integer);
  printf("Print Double %f.\n"   , num_double);
  printf("Print Float %f.\n"    , num_float);
  printf("Print Character %c.\n", txt_charachter);
  printf("Print Word %s.\n"     , txt_word);

  return 0;
}
```
