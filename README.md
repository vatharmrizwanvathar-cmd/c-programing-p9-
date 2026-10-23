# c-programing-p9-
 /* WACP to read marks scored by n students and find the average of marks */
/* demonstrate of single dimensional array */
#include<stdio.h>
int main()
{
    int n,a[25],i,total[20],m1[20],m2[20],m3[20];
    float average[20];
    printf("enter number of students:");
    scanf("%d",&n);
    for(i=0;i<=n;i++)
        {
            printf("enter the marks of 3 subjects of student %d:",i+1);
            scanf("%d%d%d",&m1[1],&m2[i],&m3[i]);
        }
    for(i=0;i<n;i++)
        {
            total[i]=m1[i]+m2[i]+m3[i];
            average[i]=(float)total[i]/3;
        }
    for(i=0;i<n;i++)
        {
            printf("\n average percentage marks of student %d is:%f", i+1, average[i]);
            if(average[i]>=35)
                printf("\n student is pass");
            else
                printf("\n student is fail");
        }
        }
        output:
        enter number of students:3
enter the marks of 3 subjects of student 1:56
67
89
enter the marks of 3 subjects of student 2:78
88
90
enter the marks of 3 subjects of student 3:89
89
90
enter the marks of 3 subjects of student 4:47
89
90

 average percentage marks of student 1 is:52.000000
 student is pass
 average percentage marks of student 2 is:75.000000
 student is pass
 average percentage marks of student 3 is:1424.666626
 student is pass
