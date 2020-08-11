#include<stdio.h>
int main()
{
    char s[100];
    int n,j,count;
    gets(s);
    for(j=0;s[j];j++);
    n=j;
    for(int i=0;i<n;i++)
    {
        count=1;
        if(s[i])
        {
            for(int j=i+1;j<n;j++)
            {
                if(s[i]==s[j])
                {
                    count++;
                    s[j]='\0';
                }
            }
            printf("count is %d %c\n",count,s[i]);
        }
    }
    return 0;
}

    
    

