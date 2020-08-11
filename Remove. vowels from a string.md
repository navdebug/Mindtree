#include <stdio.h>
int checkVowel(char ch)
{
    if(ch=='a'||ch=='A'||ch=='e'||ch=='E'||ch=='i'||ch=='I'||ch=='o'||ch=='O'||ch == 'u' || ch == 'U')
      return 1;
    else
      return 0;

}
int main()
{
    char s[100],t[100];
    gets(s);
    int c,d=0;
    for (c=0;s[c]!='\0';c++)
    {
        if (checkVowel(s[c])==0){
        t[d]=s[c];
        d++;}
    
    }
    t[d]='\0';
    strcpy(s,t);
    printf("%s",s);
    
}
