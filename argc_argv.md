# argc argv
ARGc和ARGv中的ARG指的是"参数"（外语：ARGuments, argument counter 和 argument vector ）

例子```
#include <stdio.h>

int main(int argc, char *argv[])
{
    printf("%d\n",argc);

    while(argc)
        printf("%s\n",argv[--argc]);

    printf("argv[0][1] is %c\n",argv[0][1]);
    printf("argv[0][2] is %c\n",argv[0][2]);
    printf("argv[0][3] is %c\n",argv[0][3]);

    return 0;
}

```
运行结果```
1
./demo3
argv[0][1] is /
argv[0][2] is d
argv[0][3] is e
```
