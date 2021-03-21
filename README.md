# ap2.c
homework#3
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int list[5];
    int *plist[5];

    list[0] = 10;
    list[1] = 11;

    plist[0] = (int*)malloc(sizeof(int));

    printf("list[0] \t= %d\n", list[0]);
    printf("address of list \t= %p\n", list);
    printf("address of list[0] \t= %p\n", &list[0]);
    printf("address of list + 0 \t= %p\n", list+0);
    printf("address of list + 1 \t= %p\n", list+1);
    printf("address of list + 2 \t= %p\n", list+2);
    printf("address of list + 3 \t= %p\n", list+3);
    printf("address of list + 4 \t= %p\n", list+4);
    printf("address of list[4] \t= %p\n",  &list[4]);
    //list, list[0], list+0의 주소가 다 동일하고 list+1부터 주소가 4bytes 씩 증가하다가 list+4, list[4]의 주소가 동일하다.
    printf("신태양\n");
    printf("2017038096\n");
    free(plist[0]);
}
