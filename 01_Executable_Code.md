<!--

author:   Your Name

email:    your@mail.org

version:  0.0.1

language: en

narrator: US English Female

import: https://github.com/liascript/CodeRunner
        https://github.com/LiaTemplates/AVR8js/main/README.md

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://github.com/TUBAF-IfI-LiaScript/VL_ProzeduraleProgrammierung/blob/master/04_ZeigerUndArrays.md)

# Executable Code

```c                             Pairing.c
#include <stdio.h>
#include <stdlib.h>

#define ZIELWERT 18

int main(void)
{
  int a[] = {1, 2, 5, 7, 9, 10, 12, 13, 16, 17, 18, 21, 25};
  int *ptr_left = a;
  int *ptr_right = (int *)(&a + 1) - 1;
  printf("Value left %3d right %d\n-----------------------\n", *ptr_left, * ptr_right);
  do{
    printf("Value left %3d right %d", *ptr_left, * ptr_right);
    if (*ptr_right + *ptr_left == ZIELWERT){
       printf(" -> TREFFER");
    }
    printf("\n");
    if (*ptr_right + *ptr_left >= ZIELWERT) ptr_right--;
    else ptr_left++;
  }while (ptr_right != ptr_left);
  return EXIT_SUCCESS;
}
```
@LIA.eval(`["main.c"]`, `gcc -Wall main.c -o a.out`, `./a.out`)
