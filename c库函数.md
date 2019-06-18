[TOC]


# 数学函数
函数名: abs
功 能: 求整数的绝对值
用 法: int abs(int i);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    int number = -1234;
    printf("number: %d absolute value: %d\n", number, abs(number));
    return 0;
}
```
 
函数名: acos
功 能: 反余弦函数
用 法: double acos(double x);
程序例: 
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 0.5;
    result = acos(x);
    printf("The arc cosine of %lf is %lf\n", x, result);
    return 0;
}
```
函数名: asin
功 能: 反正弦函数
用 法: double asin(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 0.5;
    result = asin(x);
    printf("The arc sin of %lf is %lf\n", x, result);
    return(0);
}
```
函数名: atan
功 能: 反正切函数
用 法: double atan(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 0.5;
    result = atan(x);
    printf("The arc tangent of %lf is %lf\n", x, result);
    return(0);
}
```
函数名: atan2
功 能: 计算Y/X的反正切值
用 法: double atan2(double y, double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 90.0, y = 45.0;
    result = atan2(y, x);
    printf("The arc tangent ratio of %lf is %lf\n", (y / x), result);
    return 0;
}
```
函数名: atan2
功 能: 计算Y/X的反正切值
用 法: double atan2(double y, double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 90.0, y = 45.0;
    result = atan2(y, x);
    printf("The arc tangent ratio of %lf is %lf\n", (y / x), result);
    return 0;
}
```
函数名: cosh
功 能: 双曲余弦函数
用 法: dluble cosh(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 0.5;
    result = cosh(x);
    printf("The hyperboic cosine of %lf is %lf\n", x, result);
    return 0;
}
```

函数名: cosh
功 能: 双曲余弦函数
用 法: dluble cosh(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 0.5;
    result = cosh(x);
    printf("The hyperboic cosine of %lf is %lf\n", x, result);
    return 0;
}
```

函数名: exp
功 能: 指数函数
用 法: double exp(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result;
    double x = 4.0;
    result = exp(x);
    printf("'e' raised to the power \
    of %lf (e ^ %lf) = %lf\n",
    x, x, result);
    return 0;
}
``` 
函数名: fabs
功 能: 返回浮点数的绝对值
用 法: double fabs(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    float number = -1234.0;
    printf("number: %f absolute value: %f\n",
    number, fabs(number));
    return 0;
}
```

函数名: floor
功 能: 向下舍入
用 法: double floor(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double number = 123.54;
    double down, up;
    down = floor(number);
    up = ceil(number);
    printf("original number %10.2lf\n",
    number);
    printf("number rounded down %10.2lf\n",
    down);
    printf("number rounded up %10.2lf\n",
    up);
    return 0;
}
```
函数名: floor
功 能: 向下舍入
用 法: double floor(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double number = 123.54;
    double down, up;
    down = floor(number);
    up = ceil(number);
    printf("original number %10.2lf\n",
    number);
    printf("number rounded down %10.2lf\n",
    down);
    printf("number rounded up %10.2lf\n",
    up);
    return 0;
}
```
函数名: frexp
功 能: 把一个双精度数分解为尾数的指数
用 法: double frexp(double value, int *eptr);
程序例:
```c
#include <math.h>
#include <stdio.h>
int main(void)
{
    double mantissa, number;
    int exponent;
    number = 8.0;
    mantissa = frexp(number, &exponent);
    printf("The number %lf is ", number);
    printf("%lf times two to the ", mantissa);
    printf("power of %d\n", exponent);
    return 0;
}
```
函数名: modf
功 能: 把数分为指数和尾数
用 法: double modf(double value, double *iptr);
程序例:
```c
#include <math.h>
#include <stdio.h>
int main(void)
{
    double fraction, integer;
    double number = 100000.567;
    fraction = modf(number, &integer);
    printf("The whole and fractional parts of %lf are %lf and %lf\n",
    number, integer, fraction);
    return 0;
}
```
函数名: pow
功 能: 指数函数(x的y次方)
用 法: double pow(double x, double y);
程序例:
```c
#include <math.h>
#include <stdio.h>
int main(void)
{
    double x = 2.0, y = 3.0;
    printf("%lf raised to %lf is %lf\n", x, y, pow(x, y));
    return 0;
}
```
函数名: rand
功 能: 随机数发生器
用 法: void rand(void);
程序例:
```c
#include <stdlib.h>
#include <stdio.h>
int main(void)
{
    int i;
    printf("Ten random numbers from 0 to 99\n\n");
    for(i=0; i<10; i++)
    printf("%d\n", rand() % 100);
    return 0;
}
```
函数名: sin
功 能: 正弦函数
用 法: double sin(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result, x = 0.5;
    result = sin(x);
    printf("The sin() of %lf is %lf\n", x, result);
    return 0;
}
```
函数名: sinh
功 能: 双曲正弦函数
用 法: double sinh(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result, x = 0.5;
    result = sinh(x);
    printf("The hyperbolic sin() of %lf is %lf\n", x, result);
    return 0;
}
```
函数名: sqrt
功 能: 计算平方根
用 法: double sqrt(double x);
程序例:
```c
#include <math.h>
#include <stdio.h>
int main(void)
{
    double x = 4.0, result;
    result = sqrt(x);
    printf("The square root of %lf is %lf\n", x, result);
    return 0;
}
```
函数名: tan
功 能: 正切函数
用 法: double tan(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result, x;
    x = 0.5;
    result = tan(x);
    printf("The tan of %lf is %lf\n", x, result);
    return 0;
}
```

函数名: tanh
功 能: 双曲正切函数
用 法: double tanh(double x);
程序例:
```c
#include <stdio.h>
#include <math.h>
int main(void)
{
    double result, x;
    x = 0.5;
    result = tanh(x);
    printf("The hyperbolic tangent of %lf is %lf\n", x, result);
    return 0;
}
```
# 字符函数和字符串函数
函数名: strcat
功 能: 字符串拼接函数
用 法: char *strcat(char *destin, char *source);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char destination[25];
    char *blank = " ", *c = "C++", *Borland = "Borland";
    strcpy(destination, Borland);
    strcat(destination, blank);
    strcat(destination, c);
    printf("%s\n", destination);
    return 0;
}
```

函数名: strchr
功 能: 在一个串中查找给定字符的第一个匹配之处\
用 法: char *strchr(char *str, char c);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char string[15];
    char *ptr, c = 'r';
    strcpy(string, "This is a string");
    ptr = strchr(string, c);
    if (ptr)
        printf("The character %c is at position: %d\n", c, ptr-string);
    else
        printf("The character was not found\n");
    return 0;
}
```

函数名: strcmp
功 能: 串比较
用 法: int strcmp(char *str1, char *str2);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char *buf1 = "aaa", *buf2 = "bbb", *buf3 = "ccc";
    int ptr;
    ptr = strcmp(buf2, buf1);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 1\n");
    else
        printf("buffer 2 is less than buffer 1\n");
    ptr = strcmp(buf2, buf3);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 3\n");
    else
        printf("buffer 2 is less than buffer 3\n");
    return 0;
}
```

函数名: strcpy
功 能: 串拷贝
用 法: char *strcpy(char *str1, char *str2);
程序例:
```c
#include <stdio.h>
#include <string.h>
int main(void)
{
    char string[10];
    char *str1 = "abcdefghi";
    strcpy(string, str1);
    printf("%s\n", string);
    return 0;
}
```

函数名: strcspn
功 能: 在串中查找第一个给定字符集内容的段
用 法: int strcspn(char *str1, char *str2);
程序例:
```c
#include <stdio.h>
#include <string.h>
#include <alloc.h>
int main(void)
{
    char *string1 = "1234567890";
    char *string2 = "747DC8";
    int length;
    length = strcspn(string1, string2);
    printf("Character where strings intersect is at position %d\n", length);
    return 0;
}
```

函数名: strdup
功 能: 将串拷贝到新建的位置处
用 法: char *strdup(char *str);
程序例:
```c
#include <stdio.h>
#include <string.h>
#include <alloc.h>
int main(void)
{
    char *dup_str, *string = "abcde";
    dup_str = strdup(string);
    printf("%s\n", dup_str);
    free(dup_str);
    return 0;
}
```

函数名: stricmp
功 能: 以大小写不敏感方式比较两个串
用 法: int stricmp(char *str1, char *str2);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char *buf1 = "BBB", *buf2 = "bbb";
    int ptr;
    ptr = stricmp(buf2, buf1);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 1\n");
    if (ptr < 0)
        printf("buffer 2 is less than buffer 1\n");
    if (ptr == 0)
        printf("buffer 2 equals buffer 1\n");
    return 0;`
}
```
函数名: strerror
功 能: 返回指向错误信息字符串的指针
用 法: char *strerror(int errnum);
程序例:
```c
#include <stdio.h>
#include <errno.h>
int main(void)
{
    char *buffer;
    buffer = strerror(errno);
    printf("Error: %s\n", buffer);
    return 0;
}
```

函数名: strcmpi
功 能: 将一个串与另一个比较, 不管大小写
用 法: int strcmpi(char *str1, char *str2);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char *buf1 = "BBB", *buf2 = "bbb";
    int ptr;
    ptr = strcmpi(buf2, buf1);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 1\n");
    if (ptr < 0)
        printf("buffer 2 is less than buffer 1\n");
    if (ptr == 0)
        printf("buffer 2 equals buffer 1\n");
    return 0;
}
```

函数名: strncmp
功 能: 串比较
用 法: int strncmp(char *str1, char *str2, int maxlen);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char *buf1 = "aaabbb", *buf2 = "bbbccc", *buf3 = "ccc";
    int ptr;
    ptr = strncmp(buf2,buf1,3);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 1\n");
    else
        printf("buffer 2 is less than buffer 1\n");
    ptr = strncmp(buf2,buf3,3);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 3\n");
    else
        printf("buffer 2 is less than buffer 3\n");
    return(0);
}
```
函数名: strncmpi
功 能: 把串中的一部分与另一串中的一部分比较, 不管大小写
用 法: int strncmpi(char *str1, char *str2);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char *buf1 = "BBBccc", *buf2 = "bbbccc";
    int ptr;
    ptr = strncmpi(buf2,buf1,3);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 1\n");
    if (ptr < 0)
        printf("buffer 2 is less than buffer 1\n");
    if (ptr == 0)
        printf("buffer 2 equals buffer 1\n");
    return 0;
}
```
函数名: strncpy
功 能: 串拷贝
用 法: char *strncpy(char *destin, char *source, int maxlen);
程序例:
```c
#include <stdio.h>
#include <string.h>
int main(void)
{
    char string[10];
    char *str1 = "abcdefghi";
    strncpy(string, str1, 3);
    string[3] = '\0';
    printf("%s\n", string);
    return 0;
}
```
函数名: strnicmp
功 能: 不注重大小写地比较两个串
用 法: int strnicmp(char *str1, char *str2, unsigned maxlen);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char *buf1 = "BBBccc", *buf2 = "bbbccc";
    int ptr;
    ptr = strnicmp(buf2, buf1, 3);
    if (ptr > 0)
        printf("buffer 2 is greater than buffer 1\n");
    if (ptr < 0)
        printf("buffer 2 is less than buffer 1\n");
    if (ptr == 0)
        printf("buffer 2 equals buffer 1\n");
    return 0;
}
```

函数名: strnset
功 能: 将一个串中的所有字符都设为指定字符
用 法: char *strnset(char *str, char ch, unsigned n);
程序例:
```c
#include <stdio.h>
#include <string.h>
int main(void)
{
    char *string = "abcdefghijklmnopqrstuvwxyz";
    char letter = 'x';
    printf("string before strnset: %s\n", string);
    strnset(string, letter, 13);
    printf("string after strnset: %s\n", string);
    return 0;
}
```
函数名: strstr
功 能: 在串中查找指定字符串的第一次出现
用 法: char *strstr(char *str1, char *str2);
程序例:
```c
#include <stdio.h>
#include <string.h>
int main(void)
{
    char *str1 = "Borland International", *str2 = "nation", *ptr;
    ptr = strstr(str1, str2);
    printf("The substring is: %s\n", ptr);
    return 0;
}
```
函数名: strtod
功 能: 将字符串转换为double型值
用 法: double strtod(char *str, char **endptr);
程序例:
```c
#include <stdio.h>
#include <stdlib.h>
int main(void)
{
    char input[80], *endptr;
    double value;
    printf("Enter a floating point number:");
    gets(input);
    value = strtod(input, &endptr);
    printf("The string is %s the number is %lf\n", input, value);
    return 0;
}
```

函数名: strtok
功 能: 查找由在第二个串中指定的分界符分隔开的单词
用 法: char *strtok(char *str1, char *str2);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    char input[16] = "abc,d";
    char *p;
    /* strtok places a NULL terminator
    in front of the token, if found */
    p = strtok(input, ",");
    if (p) printf("%s\n", p);
    /* A second call to strtok using a NULL
    as the first parameter returns a pointer
    to the character following the token */
    p = strtok(NULL, ",");
    if (p) printf("%s\n", p);
    return 0;
}
```

函数名: strtol
功 能: 将串转换为长整数
用 法: long strtol(char *str, char **endptr, int base);
程序例:
```c
#include <stdlib.h>
#include <stdio.h>
int main(void)
{
    char *string = "87654321", *endptr;
    long lnumber;
    /* strtol converts string to long integer */
    lnumber = strtol(string, &endptr, 10);
    printf("string = %s long = %ld\n", string, lnumber);
    return 0;
}
```
函数名: tolower
功 能: 把字符转换成小写字母
用 法: int tolower(int c);
程序例:
```c
#include <string.h>
#include <stdio.h>
#include <ctype.h>
int main(void)
{
    int length, i;
    char *string = "THIS IS A STRING";
    length = strlen(string);
    for (i=0; i<length; i++)
    {
    string[i] = tolower(string[i]);
    }
    printf("%s\n",string);
    return 0;
}
```
函数名: toupper
功 能: 把字符转换成大写字母
用 法: int toupper(int c);
程序例:
```c
#include <string.h>
#include <stdio.h>
#include <ctype.h>
int main(void)
{
    int length, i;
    char *string = "this is a string";
    length = strlen(string);
    for (i=0; i<length; i++)
    {
    string[i] = toupper(string[i]);
    }
    printf("%s\n",string);
    return 0;
}
```
# 输入输出函数
函数名: clearerr
功 能: 复位错误标志
用 法:void clearerr(FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    FILE *fp;
    char ch;
    /* open a file for writing */
    fp = fopen("DUMMY.FIL", "w");
    /* force an error condition by attempting to read */
    ch = fgetc(fp);
    printf("%c\n",ch);
    if (ferror(fp))
    {
    /* display an error message */
    printf("Error reading from DUMMY.FIL\n");
    /* reset the error and EOF indicators */
    clearerr(fp);
    }
    fclose(fp);
    return 0;
}
```
函数名: eof
功 能: 检测文件结束
用 法: int eof(int *handle);
程序例:
```c
#include <sys\stat.h>
#include <string.h>
#include <stdio.h>
#include <fcntl.h>
#include <io.h>
int main(void)
{
    int handle;
    char msg[] = "This is a test";
    char ch;
    /* create a file */
    handle = open("DUMMY.FIL",
    O_CREAT | O_RDWR,
    S_IREAD | S_IWRITE);
    /* write some data to the file */
    write(handle, msg, strlen(msg));
    /* seek to the beginning of the file */
    lseek(handle, 0L, SEEK_SET);
    /*
    reads chars from the file until hit EOF
    */
    do
    {
        read(handle, &ch, 1);
        printf("%c", ch);
    } while (!eof(handle));
    close(handle);
    return 0;
}
```
函数名: eof
功 能: 检测文件结束
用 法: int eof(int *handle);
程序例:
```c
#include <sys\stat.h>
#include <string.h>
#include <stdio.h>
#include <fcntl.h>
#include <io.h>
int main(void)
{
    int handle;
    char msg[] = "This is a test";
    char ch;
    /* create a file */
    handle = open("DUMMY.FIL",
    O_CREAT | O_RDWR,
    S_IREAD | S_IWRITE);
    /* write some data to the file */
    write(handle, msg, strlen(msg));
    /* seek to the beginning of the file */
    lseek(handle, 0L, SEEK_SET);
    /*
    reads chars from the file until hit EOF
    */
    do
    {
    read(handle, &ch, 1);
    printf("%c", ch);
    } while (!eof(handle));
    close(handle);
    return 0;
}
```
函数名: exec...
功 能: 装入并运行其它程序的函数
用 法: int execl(char *pathname, char *arg0, arg1, ..., argn, NULL);
int execle(char *pathname, char *arg0, arg1, ..., argn, NULL,
char *envp[]);
int execlp(char *pathname, char *arg0, arg1, .., NULL);
int execple(char *pathname, char *arg0, arg1, ..., NULL,
char *envp[]);
int execv(char *pathname, char *argv[]);
int execve(char *pathname, char *argv[], char *envp[]);
int execvp(char *pathname, char *argv[]);
int execvpe(char *pathname, char *argv[], char *envp[]);
程序例:
```c
/* execv example */
#include <process.h>
#include <stdio.h>
#include <errno.h>
void main(int argc, char *argv[])
{
    int i;
    printf("Command line arguments:\n");
    for (i=0; i<argc; i++)
    printf("[%2d] : %s\n", i, argv[i]);
    printf("About to exec child with arg1 arg2 ...\n");
    execv("CHILD.EXE", argv);
    perror("exec error");
    exit(1);
}
```
函数名: fclose
功 能: 关闭一个流
用 法: int fclose(FILE *stream);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    FILE *fp;
    char buf[11] = "0123456789";
    /* create a file containing 10 bytes */
    fp = fopen("DUMMY.FIL", "w");
    fwrite(&buf, strlen(buf), 1, fp);
    /* close the file */
    fclose(fp);
    return 0;
}
```

函数名: feof
功 能: 检测流上的文件结束符
用 法: int feof(FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    FILE *stream;
    /* open a file for reading */
    stream = fopen("DUMMY.FIL", "r");
    /* read a character from the file */
    fgetc(stream);
    /* check for EOF */
    if (feof(stream))
    printf("We have reached end-of-file\n");
    /* close the file */
    fclose(stream);
    return 0;
}
```
函数名: fgetc
功 能: 从流中读取字符
用 法: int fgetc(FILE *stream);
程序例:
```c
#include <string.h>
#include <stdio.h>
#include <conio.h>
int main(void)
{
    FILE *stream;
    char string[] = "This is a test";
    char ch;
    /* open a file for update */
    stream = fopen("DUMMY.FIL", "w+");
    /* write a string into the file */
    fwrite(string, strlen(string), 1, stream);
    /* seek to the beginning of the file */
    fseek(stream, 0, SEEK_SET);
    do
    {
        /* read a char from the file */
        ch = fgetc(stream);
        /* display the character */
        putch(ch);
    } while (ch != EOF);
    fclose(stream);
    return 0;
}
```
函数名: fgets
功 能: 从流中读取一字符串
用 法: char *fgets(char *string, int n, FILE *stream);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    FILE *stream;
    char string[] = "This is a test";
    char msg[20];
    /* open a file for update */
    stream = fopen("DUMMY.FIL", "w+");
    /* write a string into the file */
    fwrite(string, strlen(string), 1, stream);
    /* seek to the start of the file */
    fseek(stream, 0, SEEK_SET);
    /* read a string from the file */
    fgets(msg, strlen(string)+1, stream);
    /* display the string */
    printf("%s", msg);
    fclose(stream);
    return 0;
}
```

函数名: fopen
功 能: 打开一个流
用 法: FILE *fopen(char *filename, char *type);
程序例:
```c
#include <stdlib.h>
#include <stdio.h>
#include <dir.h>
int main(void)
{
    char *s;
    char drive[MAXDRIVE];
    char dir[MAXDIR];
    char file[MAXFILE];
    char ext[MAXEXT];
    int flags;
    s=getenv("COMSPEC"); /* get the comspec environment parameter */
    flags=fnsplit(s,drive,dir,file,ext);
    printf("Command processor info:\n");
    if(flags & DRIVE)
    printf("\tdrive: %s\n",drive);
    if(flags & DIRECTORY)
    printf("\tdirectory: %s\n",dir);
    if(flags & FILENAME)
    printf("\tfile: %s\n",file);
    if(flags & EXTENSION)
    printf("\textension: %s\n",ext);
    return 0;
}
```
函数名: fprintf
功 能: 传送格式化输出到一个流中
用 法: int fprintf(FILE *stream, char *format[, argument,...]);
程序例:
```c
/* Program to create backup of the
AUTOEXEC.BAT file */
#include <stdio.h>
int main(void)
{
    FILE *in, *out;
    if ((in = fopen("\\AUTOEXEC.BAT", "rt"))== NULL)
    {
        fprintf(stderr, "Cannot open input \
        file.\n");
        return 1;
    }
    if ((out = fopen("\\AUTOEXEC.BAK", "wt"))== NULL)
    {
        fprintf(stderr, "Cannot open output \
        file.\n");
        return 1;
    }
    while (!feof(in))
        fputc(fgetc(in), out);
    fclose(in);
    fclose(out);
    return 0;
}
```
函数名: fputc
功 能: 送一个字符到一个流中
用 法: int fputc(int ch, FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    char msg[] = "Hello world";
    int i = 0;
    while (msg[i])
    {
        fputc(msg[i], stdout);
        i++;
    }
    return 0;
}
```
函数名: fputs
功 能: 送一个字符到一个流中
用 法: int fputs(char *string, FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    /* write a string to standard output */
    fputs("Hello world\n", stdout);
    return 0;
}
```

函数名: fread
功 能: 从一个流中读数据
用 法: int fread(void *ptr, int size, int nitems, FILE *stream);
程序例:
```c
#include <string.h>
#include <stdio.h>
int main(void)
{
    FILE *stream;
    char msg[] = "this is a test";
    char buf[20];
    if ((stream = fopen("DUMMY.FIL", "w+")) == NULL)
    {
        fprintf(stderr,
        "Cannot open output file.\n");
        return 1;
    }
    /* write some data to the file */
    fwrite(msg, strlen(msg)+1, 1, stream);
    /* seek to the beginning of the file */
    fseek(stream, SEEK_SET, 0);
    /* read the data and display it */
    fread(buf, strlen(msg)+1, 1, stream);
    printf("%s\n", buf);
    fclose(stream);
    return 0;
}
```
函数名: fscanf
功 能: 从一个流中执行格式化输入
用 法: int fscanf(FILE *stream, char *format[,argument...]);
程序例:
```c
#include <stdlib.h>
#include <stdio.h>
int main(void)
{
    int i;
    printf("Input an integer: ");
    /* read an integer from the
    standard input stream */
    if (fscanf(stdin, "%d", &i))
        printf("The integer read was: %i\n", i);
    else
    {
        fprintf(stderr, "Error reading an \
        integer from stdin.\n");
        exit(1);
    }
    return 0;
}
```

函数名: fseek
功 能: 重定位流上的文件指针
用 法: int fseek(FILE *stream, long offset, int fromwhere);
程序例:
```c
#include <stdio.h>
long filesize(FILE *stream);
int main(void)
{
    FILE *stream;
    stream = fopen("MYFILE.TXT", "w+");
    fprintf(stream, "This is a test");
    printf("Filesize of MYFILE.TXT is %ld bytes\n", filesize(stream));
    fclose(stream);
    return 0;
}
long filesize(FILE *stream)
{
    long curpos, length;
    curpos = ftell(stream);
    fseek(stream, 0L, SEEK_END);
    length = ftell(stream);
    fseek(stream, curpos, SEEK_SET);
    return length;
}
```

函数名: ftell
功 能: 返回当前文件指针
用 法: long ftell(FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    FILE *stream;
    stream = fopen("MYFILE.TXT", "w+");
    fprintf(stream, "This is a test");
    printf("The file pointer is at byte \
    %ld\n", ftell(stream));
    fclose(stream);
    return 0;
}
```

函数名: fwrite
功 能: 写内容到流中
用 法: int fwrite(void *ptr, int size, int nitems, FILE *stream);
程序例:
```c
#include <stdio.h>
struct mystruct
{
    int i;
    char ch;
    };
int main(void)
{
    FILE *stream;
    struct mystruct s;
    if ((stream = fopen("TEST.$$$", "wb")) == NULL) /* open file TEST.$$$ */
    {
    fprintf(stderr, "Cannot open output file.\n");
    return 1;
    }
    s.i = 0;
    s.ch = 'A';
    fwrite(&s, sizeof(s), 1, stream); /* write struct s to file */
    fclose(stream); /* close file */
    return 0;
}
``` 
函数名: getc
功 能: 从流中取字符
用 法: int getc(FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    char ch;
    printf("Input a character:");
    /* read a character from the
    standard input stream */
    ch = getc(stdin);
    printf("The character input was: '%c'\n",
    ch);
    return 0;
}
```

函数名: getchar
功 能: 从stdin流中读字符
用 法: int getchar(void);
程序例:
```c
#include <stdio.h>
int main(void)
{
    int c;
    /* Note that getchar reads from stdin and
    is line buffered; this means it will
    not return until you press ENTER. */
    while ((c = getchar()) != '\n')
    printf("%c", c);
    return 0;
}
```
函数名: open
功 能: 打开一个文件用于读或写
用 法: int open(char *pathname, int access[, int permiss]);
程序例:
```c
#include <string.h>
#include <stdio.h>
#include <fcntl.h>
#include <io.h>
int main(void)
{
    int handle;
    char msg[] = "Hello world";
    if ((handle = open("TEST.$$$", O_CREAT | O_TEXT)) == -1)
    {
        perror("Error:");
        return 1;
    }
    write(handle, msg, strlen(msg));
    close(handle);
    return 0;
}
```
函数名: printf
功 能: 产生格式化输出的函数
用 法: int printf(char *format...);
程序例:
```c
#include <stdio.h>
#include <string.h>
#define I 555
#define R 5.5
int main(void)
{
    int i,j,k,l;
    char buf[7];
    char *prefix = buf;
    char tp[20];
    printf("prefix 6d 6o 8x 10.2e "
    "10.2f\n");
    strcpy(prefix,"%");
    for (i = 0; i < 2; i++)
    {
        for (j = 0; j < 2; j++)
            for (k = 0; k < 2; k++)
                for (l = 0; l < 2; l++)
                {
                    if (i==0) strcat(prefix,"-");
                    if (j==0) strcat(prefix,"+");
                    if (k==0) strcat(prefix,"#");
                    if (l==0) strcat(prefix,"0");
                    printf("%5s |",prefix);
                    strcpy(tp,prefix);
                    strcat(tp,"6d |");
                    printf(tp,I);
                    strcpy(tp,"");
                    strcpy(tp,prefix);
                    strcat(tp,"6o |");
                    printf(tp,I);
                    strcpy(tp,"");
                    strcpy(tp,prefix);
                    strcat(tp,"8x |");
                    printf(tp,I);
                    strcpy(tp,"");
                    strcpy(tp,prefix);
                    strcat(tp,"10.2e |");
                    printf(tp,R);
                    strcpy(tp,prefix);
                    strcat(tp,"10.2f |");
                    printf(tp,R);
                    printf(" \n");
                    strcpy(prefix,"%"); 
                }
    }
    return 0;
}
```
函数名: putc
功 能: 输出一字符到指定流中
用 法: int putc(int ch, FILE *stream);
程序例:
```c
#include <stdio.h>
int main(void)
{
    char msg[] = "Hello world\n";
    int i = 0;
    while (msg[i])
    putc(msg[i++], stdout);
    return 0;
}
```

函数名: putchar
功 能: 在stdout上输出字符
用 法: int putchar(int ch);
程序例:
```c
#include <stdio.h>
/* define some box-drawing characters */
#define LEFT_TOP 0xDA
#define RIGHT_TOP 0xBF
#define HORIZ 0xC4
#define VERT 0xB3
#define LEFT_BOT 0xC0
#define RIGHT_BOT 0xD9
int main(void)
{
    char i, j;
    /* draw the top of the box */
    putchar(LEFT_TOP);
    for (i=0; i<10; i++)
        putchar(HORIZ);
    putchar(RIGHT_TOP);
    putchar('\n');
    /* draw the middle */
    for (i=0; i<4; i++)
    {
        putchar(VERT);
        for (j=0; j<10; j++)
        putchar(' ');
        putchar(VERT);
        putchar('\n');
    }
    /* draw the bottom */
    putchar(LEFT_BOT);
    for (i=0; i<10; i++)
        putchar(HORIZ);
    putchar(RIGHT_BOT);
    putchar('\n');
    return 0;
}
```
函数名: puts
功 能: 送一字符串到流中
用 法: int puts(char *string);
程序例:
```c
#include <stdio.h>
int main(void)
{
    char string[] = "This is an example output string\n";
    puts(string);
    return 0;
}
```
函数名: read
功 能: 从文件中读
用 法: int read(int handle, void *buf, int nbyte);
程序例:
```c
#include <stdio.h>
#include <io.h>
#include <alloc.h>
#include <fcntl.h>
#include <process.h>
#include <sys\stat.h>
int main(void)
{
    void *buf;
    int handle, bytes;
    buf = malloc(10);
    /*
    Looks for a file in the current directory named TEST.$$$ and attempts
    to read 10 bytes from it. To use this example you should create the
    file TEST.$$$
    */
    if ((handle = open("TEST.$$$", O_RDONLY | O_BINARY, S_IWRITE | S_IREAD)) == -1)
    {
        printf("Error Opening File\n");
        exit(1);
    }
    if ((bytes = read(handle, buf, 10)) == -1) {
        printf("Read Failed.\n");
        exit(1);
    }
    else {
        printf("Read: %d bytes read.\n", bytes);
    }
    return 0;
}
```
函数名: rename
功 能: 重命名文件
用 法: int rename(char *oldname, char *newname);
程序例:
```c
#include <stdio.h>
int main(void)
{
    char oldname[80], newname[80];
    /* prompt for file to rename and new name */
    printf("File to rename: ");
    gets(oldname);
    printf("New name: ");
    gets(newname);
    /* Rename the file */
    if (rename(oldname, newname) == 0)
        printf("Renamed %s to %s.\n", oldname, newname);
    else
        perror("rename");
    return 0;
}
```
函数名: rewind
功 能: 将文件指针重新指向一个流的开头
用 法: int rewind(FILE *stream);
程序例:
```c
#include <stdio.h>
#include <dir.h>
int main(void)
{
    FILE *fp;
    char *fname = "TXXXXXX", *newname, first;
    newname = mktemp(fname);
    fp = fopen(newname,"w+");
    fprintf(fp,"abcdefghijklmnopqrstuvwxyz");
    rewind(fp);
    fscanf(fp,"%c",&first);
    printf("The first character is: %c\n",first);
    fclose(fp);
    remove(newname);
    return 0;
}
```
函数名: scanf
功 能: 执行格式化输入
用 法: int scanf(char *format[,argument,...]);
程序例:
```c
#include <stdio.h>
#include <conio.h>
int main(void)
{
    char label[20];
    char name[20];
    int entries = 0;
    int loop, age;
    double salary;
    struct Entry_struct
    {
        char name[20];
        int age;
        float salary;
    } entry[20];
    /* Input a label as a string of characters restricting to 20 characters */
    printf("\n\nPlease enter a label for the chart: ");
    scanf("%20s", label);
    fflush(stdin); /* flush the input stream in case of bad input */
    /* Input number of entries as an integer */
    printf("How many entries will there be? (less than 20) ");
    scanf("%d", &entries);
    fflush(stdin); /* flush the input stream in case of bad input */
    /* input a name restricting input to only letters upper or lower case */
    for (loop=0;loop<entries;++loop)
    {
        printf("Ent ry %d\n", loop);
        printf(" Name : ");
        scanf("%[A-Za-z]", entry[loop].name);
        fflush(stdin); /* flush the input stream in case of bad input */
        /* input an age as an integer */
        printf(" Age : ");
        scanf("%d", &entry[loop].age);
        fflush(stdin); /* flush the input stream in case of bad input */
        /* input a salary as a float */
        printf(" Salary : ");
        scanf("%f", &entry[loop].salary);
        fflush(stdin); /* flush the input stream in case of bad input */
    }
    /* Input a name, age and salary as a string, integer, and double */
    printf("\nPlease enter your name, age and salary\n");
    scanf("%20s %d %lf", name, &age, &salary);

    /* Print out the data that was input */
    printf("\n\nTable %s\n",label);
    printf("Compiled by %s age %d $%15.2lf\n", name, age, salary);
    printf("-----------------------------------------------------\n");
    for (loop=0;loop<entries;++loop)
        printf("%4d | %-20s | %5d | %15.2lf\n",
        loop + 1,
        entry[loop].name,
        entry[loop].age,
        entry[loop].salary);
    printf("-----------------------------------------------------\n");
    return 0;
}
```
# 动态存储分配函数
函数名: calloc
功 能: 分配主存储器
用 法: void *calloc(size_t nelem, size_t elsize);
程序例:
```c
#include <stdio.h>
#include <alloc.h>
int main(void)
{
    char *str = NULL;
    /* allocate memory for string */
    str = calloc(10, sizeof(char));
    /* copy "Hello" into string */
    strcpy(str, "Hello");
    /* display string */
    printf("String is %s\n", str);
    /* free memory */
    free(str);
    return 0;
}
```

函数名: free
功 能: 释放已分配的块
用 法: void free(void *ptr);
程序例:
```c
#include <string.h>
#include <stdio.h>
#include <alloc.h>
int main(void)
{
    char *str;
    /* allocate memory for string */
    str = malloc(10);
    /* copy "Hello" to string */
    strcpy(str, "Hello");
    /* display string */
    printf("String is %s\n", str);
    /* free memory */
    free(str);
    return 0;
}
```
函数名: malloc
功 能: 内存分配函数
用 法: void *malloc(unsigned size);
程序例:
```c
#include <stdio.h>
#include <string.h>
#include <alloc.h>
#include <process.h>
int main(void)
{
    char *str;
    /* allocate memory for string */
    /* This will generate an error when compiling */
    /* with C++, use the new operator instead. */
    if ((str = malloc(10)) == NULL)
    {
        printf("Not enough memory to allocate buffer\n");
        exit(1); /* terminate program if out of memory */
    }
    /* copy "Hello" into string */
    strcpy(str, "Hello");
    /* display string */
    printf("String is %s\n", str);
    /* free memory */
    free(str);
    return 0;
}
```

函数名: realloc
功 能: 重新分配主存
用 法: void *realloc(void *ptr, unsigned newsize);
程序例:
```c
#include <stdio.h>
#include <alloc.h>
#include <string.h>
int main(void)
{
    char *str;
    /* allocate memory for string */
    str = malloc(10);
    /* copy "Hello" into string */
    strcpy(str, "Hello");
    printf("String is %s\n Address is %p\n", str, str);
    str = realloc(str, 20);
    printf("String is %s\n New address is %p\n", str, str);
    /* free memory */
    free(str);
    return 0;
}
```