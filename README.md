# Milestone-5-Final-Application-Release
#include <stdio.h>
int main()
{
    /* Pointer to the file */
    FILE* fp1;
    /* Character variable to read the content of file */
    char c;

    /* Opening a file in r mode*/
    fp1 = fopen_s("C:\\myfiles\\newfile.txt", "r", 1);

    /* Infinite loop –I have used break to come out of the loop*/
    while (1)
    {
        c = fgetc(fp1);
        if (c == EOF)
            break;
        else
            printf_s("%c", c);
    }
    fclose_s(fp1);
    return 0;
}
