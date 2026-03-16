//To enter yuour name using string 
#include<stdio.h>
int main()
{
char name[20];
printf("Enter your name: ");
scanf("%s",name);
printf("Your name is %s",name);
return 0;
}

//To fidn the length of the string
#include<stdio.h>
#include<string.h>
int main()
{
char str[50]="RAHULSAI";
int len=strlen(str);
printf("Length of the string:%d",len);
return 0;
}

//To find the lowercase,uppercase and string reverse
#include<stdio.h>
#include<string.h>
int main()
{
char str[50]="RAHULSAI";
char str1[50]="rahulsai";
char str2[50]="RAHULSAI";
strlwr(str);
strupr(str1);
strrev(str2);
printf("In uppercase:%s\n",str);
printf("In lowercase:%s\n",str1);
printf("In reverse:%s",str2);
return 0;
}

//To compare two strings
#include<stdio.h>
#include<string.h>
int main()
{
char s1[20]="RAHUL";
char s2[20]="VIRAT";
if(strcmp(s1,s2)==0){
printf("s1 and s2 are equal");
}
else{
printf("s1 and s2 are not equal");
}
return 0;
}

//To concatenation a string
#include<stdio.h>
int main()
{
char s1[50]="RAHUL";
char s2[30]="VIRAT";
strcat(s1,s2);
printf("After concatenation:%s",s1);
return 0;
}

//To copy a string into another
#include<stdio.h>
int main()
{
char s1[30]="rahul";
char s2[30]="prabhas";
strcpy(s1,s2);
printf("Output string copy:%s",s1);
return 0;
}

//To find the string lenght without using string ffunction
#include<stdio.h>
int main()
{
char str[30]="RAHUL";
//gets [str]
int i=0,len=0;
while (str[i]!='\0'){
len++;
i++;
}
printf("Length of the string:%d",str);
return 0;
}

//To count the no of words in the given statement
#include<stdio.h>
#include<string.h>
int main()
{
char [50]="RAHUL";
int i; count=1;
for (i=0;str[i]!='\0';i++){
if(str[i]==' '){
count++;
}
}
printf("No.of words:%d",count);
return 0;
}

//To concatenate without using string function
#include<stdio.h>
int main()
{
char str1[20]="RAHUL";
char str2[20]="SAI";
int i=0,j=0;
while(str1[i]!='\0'){
i++;}
str1[i]=str2[j];
while (str2[j]!='\0'){
i++;
j++;
}
str1[i]='\0';
printf("Concatenated string=%s",str1);
return 0;
}

//To convert to uppercase without using str function
#include<stdio.h>
int main()
{
char str[20]="rahulsai"
int i=0;
while(str[i]!='\0'){
if (str[i]>='a'&&str[i]<='z'){
str[i]=str[i]-32;
}
i++;
}
printf(str);
return 0;
}

//to convert into lower case letters without uing the the string fuctions
#include<stdio.h>
int main()
{
int i=0;
char str[20]="RAHULSAI";
int i=0;
while (str[i]>='A'&&str[i]<='Z'){
str[i]=str[i]+32;
}
i++;
printf(str);
return 0;
}
//to reverse a string without using string function
#include<stdio.h>
int main()
{
char str[10]="RAHUL";
char rev[10];
l=strlen(str);
for(i=l-1;i>=0;i--){
rev[j]=str[i];
j++;
}
rev[j]='\0';
printf("reversed string% s",rev);
return 0;
}
#include<stdio.h>
#include<string.h>
void main()
{
char str[10]="malayalam";
int,length,flag=0;
length=strlen(str);
for(i=0;i<lenght;i++){
if(str[i]!=str[length-i-1]){
flag=1;
break;
}
}
if(flag==1){
printf("%d is not a pal",str);
}else{
printf("%d is pal,str);
//count no.of consonants and vowels in a sentence
#include<stdio.h>
void main()
{
char sentence[30]="rahul sai";
int i,vowels=0;consonants=0;
char ch;
for(i=0;sentence[i]!=0;'0\';i++){
ch=sentence[i];
if(ch='a'&& ch<='z'){
if(ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u')
vowels++;
else
consonants++;
}
}printf("d%\n,vowels);
printf("d%\n,vowels);
}
//to remove duplicate
#include<stdio.h>
int main()
{
char star[100]="rahul"
int i,j,k;
for(i=0;str[i]!='\o';i++)
{
for(j=i+1;str[j]!='\o';j++)
{
if(str[i]==str[j]){
for(k=j;str[k]!='o\';k++){
str[k]=str[k+1];
}
j--;
}
}
}
printf("string after remoivng duplicates:%s",str);
return 0;
}

