#include <stdio.h>
#include <string.h>

int main()
{
    char str1[50] = "RAHUL SAI";
    char str2[50] = " CLOUD";
    char temp[50];
    int i, length = 0, words = 1, vowels = 0, consonants = 0;

    printf("Original String: %s\n\n", str1);

    //1. strlen
    printf("1. Length using strlen: %lu\n", strlen(str1));

    //2. Lowercase
    strcpy(temp, str1);
    for(i=0; temp[i]; i++)
        if(temp[i] >= 'A' && temp[i] <= 'Z')
            temp[i] = temp[i] + 32;
    printf("2. Lowercase: %s\n", temp);

    //Uppercase
    strcpy(temp, str1);
    for(i=0; temp[i]; i++)
        if(temp[i] >= 'a' && temp[i] <= 'z')
            temp[i] = temp[i] - 32;
    printf("Uppercase: %s\n", temp);

    //Reverse
    strcpy(temp, str1);
    int len = strlen(temp);
    for(i=len-1;i>=0;i--)
        printf("%c", temp[i]);
    printf("\n");

    //3. String conversion (copy)
    strcpy(temp,str1);
    printf("3. String copied: %s\n", temp);

    //4. strcat
    char concat[100];
    strcpy(concat,str1);
    strcat(concat,str2);
    printf("4. strcat result: %s\n", concat);

    //5. strcpy
    char copy[50];
    strcpy(copy,str1);
    printf("5. strcpy result: %s\n", copy);

    //6. Length without strlen
    for(i=0; str1[i]!='\0'; i++)
        length++;
    printf("6. Length without strlen: %d\n", length);

    //7. Count words without strlen
    for(i=0; str1[i]!='\0'; i++)
        if(str1[i]==' ')
            words++;
    printf("7. Word count without strlen: %d\n", words);

    //8. Number of words
    printf("8. Number of words: %d\n", words);

    //9. Concatenate without strcat
    char a[100] = "RAHUL ";
    char b[50] = "SAI";
    int j=0;
    for(i=0; a[i]!='\0'; i++);
    while(b[j]!='\0')
    {
        a[i]=b[j];
        i++;
        j++;
    }
    a[i]='\0';
    printf("9. Concatenate without function: %s\n", a);

    //10. Lower to Upper without function
    char lower[50] = "rahul";
    for(i=0; lower[i]; i++)
        if(lower[i]>='a' && lower[i]<='z')
            lower[i]=lower[i]-32;
    printf("10. Lower to Upper: %s\n", lower);

    //11. Upper to Lower without function
    char upper[50] = "RAHUL";
    for(i=0; upper[i]; i++)
        if(upper[i]>='A' && upper[i]<='Z')
            upper[i]=upper[i]+32;
    printf("11. Upper to Lower: %s\n", upper);

    //12. Reverse without function
    char rev[50] = "RAHUL";
    int l=0;
    while(rev[l]!='\0')
        l++;
    printf("12. Reverse without function: ");
    for(i=l-1;i>=0;i--)
        printf("%c",rev[i]);
    printf("\n");

    //13. Palindrome
    char p[50] = "MADAM";
    int flag=0;
    int n=strlen(p);
    for(i=0;i<n/2;i++)
        if(p[i]!=p[n-i-1])
            flag=1;
    if(flag==0)
        printf("13. Palindrome\n");
    else
        printf("13. Not Palindrome\n");

    //14. Count vowels and consonants
    char s[50] = "RAHUL";
    for(i=0;s[i]!='\0';i++)
    {
        if(s[i]=='A'||s[i]=='E'||s[i]=='I'||s[i]=='O'||s[i]=='U'||
           s[i]=='a'||s[i]=='e'||s[i]=='i'||s[i]=='o'||s[i]=='u')
            vowels++;
        else if(s[i]!=' ')
            consonants++;
    }
    printf("14. Vowels: %d Consonants: %d\n", vowels, consonants);

    return 0;
}
