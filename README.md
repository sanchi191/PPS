
Write a program to print calculatorvoid main()
{
int num1, num2, res;
char op;
printf(“Enter the First number”);
scanf("%d", &num1);
printf(“Enter the second number”);
scanf("%d", &num2);
printf(“What operation do you want to perform /
/s for sum, b for subtract, d for divide , m for multiply “);
scanf(” %c”,&op);

switch(op)
{
case ‘s’:
res = num1 + num2;
printf(“The sum of the chosen number is %d”, res );
break;

    case 'b':
            res = num1 - num2;
            printf("The difference of the chosen number is %d", res );
    break;  

    case 'd':
            res = num1 / num2;
            printf("The ratio of the chosen number is %d", res );
    break;

    case 'm':
            res = num1 * num2;
            printf("The product of the chosen number is %d\n", res );
    break;

    default:
            printf("Get your eyes checked by Doctor ");     
    break;
    }

}
OUTPUT:
Enter the First number:23
Enter the second number:45
What operation do you want to perform s for sum, b for subtract, d for divide , m for multiply m
The product of the chosen number is :1035Write a program for bubble sorting#include<stdio.h>
int main()
{
int a[20],n,i,k,temp;
printf(“Enter the size of array”);
scanf("%d",&n);
printf(“Enter %d no. of arrays”);
for(i=0;i<n;i++)
scanf("%d",&a[i]);
for(k=0;k<n-1;k++)
{
for(i=0;i<n-k-1;i++)
{
if(a[i]>a[i+1])
{
temp=a[i];
a[i]=a[i+1];
a[i+1]=temp;
}
}
}
printf(“Array elements after sorting \n”);
for(i=0;i<n;i++)
printf("%d",a[i]);
return(0);
}
output
Enter the size of array6
Enter 1 no. of arrays9
4
6
7
23
45
Array elements after sorting
46792345

Write a program for binary search
#include <stdio.h>
 int main()
{
   int c, first, last, middle, n, search, array[100];
 
   printf(“Enter number of elements\n”);
   scanf("%d",&n);
 
   printf(“Enter %d integers\n”, n);
 
   for (c = 0; c < n; c++)
      scanf("%d",&array[c]);
 
   printf(“Enter value to find\n”);
   scanf("%d", &search);
 
   first = 0;
   last = n - 1;
   middle = (first+last)/2;
 
   while (first <= last) {
      if (array[middle] < search)
         first = middle + 1;    
      else if (array[middle] == search) {
         printf("%d found at location %d.\n", search, middle+1);
         break;
      }
      else
         last = middle - 1;
 
      middle = (first + last)/2;
   }
   if (first > last)
      printf(“Not found! %d isn’t present in the list.\n”, search);
 
   return 0;

Program to Find factorial of a number using recursion:
int count = 1, num;
int multiply(int num);

int main(){
printf(“Welcome to the program to find factorial by recursion”);
printf(“Write the number:\n”);
scanf("%d",&num);
multiply(num);
printf(“The facorial is %d”,count);
}

int multiply(int num){
count = count * num;
if(num>1){
multiply(num - 1);
}
return count;}
OUTPUT:
Welcome to the program to find factorial by recursionWrite the number:
8
The facorial is 40320

Program of FizzBuzz:
int num;
int main(){
printf(“Welcome to the Fizz Buzz Program”);
printf(“Enter The number”);
scanf("%d",&num);
if (num%3 == 0 && num%5 !=0)
printf(“Fizz”);
if (num%3 != 0 && num%5 == 0)
printf(“Buzz”);
if (num%3 == 0 && num%5 == 0)
printf(“FizzBuzz”);
}
OUTPUT:
Welcome to the Fizz Buzz Program
Enter The number:45
FizzBuzz

Write a program to find sum of first 100 numbers
#include<stdio.h>
int main()
{
int sum=0,number;
number=1;
while(number<=100)
{
sum+=number;
number++;
}
printf(“sum of first 100 positive no. is %d”,sum);
return(0);
}
Write a program to find greater of two numbers
#include<stdio.h>
int main()
{
int a,b;
printf(“Enter any two no.”);
scanf("%d%d",&a,&b);
if(a>b)
printf(“a is greater”);
else
printf(“b is greater”);
return(0);
}

Write a program to find greater of three numbers
#include<stdio.h>
int biggestnumber(int a,int b,int c);
int main()
{
int n1,n2,n3,result;
printf(“Enter three numbers”,n1,n2,n3);
scanf("%d%d%d",&n1,&n2,&n3);
result=biggestnumber(n1,n2,n3);
printf(“biggest number is %d”,result);
return(0);
}
int biggestnumber(int a,int b,int c)
{
if(a>b)
{
if(a>c)
return a;
else
return c;
}
else
if(b>c)
return b;
else
return c;
}

Write a program to find GCD of numbers
#include<stdio.h>
int main()
{
int m,n,r=1;
printf(“Enter the value of m and n”);
scanf("%d %d",&m,&n);
while(r!=0)
{
r=n%m;
n=m;
m=r;
}
printf("\n GCD=%d",n);
return(0);
}

Program to check a Leap year
int year;
int main(){
printf(“Hi welcome to the program that checks the leap year”);
printf(“Please enter the value of the year\n”);
scanf("%d",&year);
if (year%4 == 0)
printf(“The year is a leap year”);
else
printf(“The year is not a leap year”);

}
OUTPUT:
Hi welcome to the program that checks the leap yearPlease enter the value of the year
2005
The year is not a leap year

Write a program for linear search
#include<stdio.h>
int main()
{
int array[100],n,c,search;
printf(“Enter the number of elements”);
scanf("%d",&n);
for(c=0;c<n;c++)
scanf("%d",&array[c]);
printf(“Enter the element to search”);
scanf("%d",&search);
for(c=0;c<n;c++)
{
if(array[c]search)
{
printf(“element is found”);
printf("%d is the location",c+1);
break;
}
}
if(cn)
printf("%d element is not found\n",search);
return(0);
}

Program to add to Matrix:

int a[3][3], b[3][3],c[3][3], i ,j;
int main(){
printf(“Welcome to the Matrix Program”);

printf(“Enter the value of matrix A”);
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&a[i][j]);
}}

printf(“Enter the value of matrix B”);
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&b[i][j]);
}}

printf(“You have entered all the values of the matrix\n”);
printf(“Now the program is displaying the addition of matrix”);

for(i=0;i<3;i++){
for(j=0;j<3;j++){
c[i][j] = b[i][j] + a[i][j];
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",c[i][j]);
}
printf("\n");}

}
OUTPUT:
Welcome to the Matrix ProgramEnter the value of matrix A
23
67
12
89
23
78
12
65
23
Enter the value of matrix B45
67
89
23
62
48
69
52
84
You have entered all the values of the matrix
Now the program is displaying the addition of matrix
68 134 101
112 85 126
81 117 107

21)Program to Display Transpose of Matrix:

int a[3][3],c[3][3], i ,j;
int main(){
printf(“Welcome to the Matrix Transpose Program”);

printf(“Enter the value of matrix”);
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&a[i][j]);
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",a[i][j]);
}

printf(“You have entered all the values of the matrix\n”);
printf(“Now the program is displaying the transpose of matrix\n”);

for(i=0;i<3;i++){
for(j=0;j<3;j++){
c[j][i] = a[i][j];
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",c[i][j]);
}
printf("\n");}

}
}
OUTPUT:
Welcome to the Matrix Transpose ProgramEnter the value of matrix34
34
56
625
536
75
68
97
07
You have entered all the values of the matrix
Now the program is displaying the transpose of matrix
34 625 68
34 536 97
56 75 7

Write a program to find sum of digits of number
#include<stdio.h>
int main()
{
int n,sum=0,m;
printf(“Enter a number:”);
scanf("%d",&n);
while(n>0)
{
m=n%10;
sum=sum+m;
n=n/10;
}
printf(“Sum is=%d”,sum);
return 0;
}

Output:

Enter a number:654
Sum is=15

Enter a number:123
Sum is=6

Program to check if a number is Palindrome

int x,num, num_loop,rev= 0;
int main(){
printf(“Welcome to the palindrome function\n”);
printf(“Enter the number:\n”);
scanf("%d",&num);
num_loop = num;
while(num_loop > 1){
x = num_loop % 10;
rev = rev * 10 +x;
num_loop = num_loop/10;
}
if (rev == num)
printf(“oh yes ! You wrote a palindrome number”);
else
printf(“sorry the number is not a palindrome”);
}
OUTPUT:
Welcome to the palindrome function
Enter the number:
234565432
oh yes ! You wrote a palindrome number

Program to swap two numbers by call by value
void swap(int a,int b);
void main()Write a program to add two numbers#include<stdio.h>
int addnumbers(int a,int b);
int main()
{
int n1,n2,sum;
printf(“Enter the two numbers”);
scanf("%d%d",&n1,&n2);
sum=addnumbers( n1, n2);
printf("\nsum of two numbers is %d",sum);
return(0);
}
int addnumbers(int a,int b)
{
int c;
c=a+b;
return©;
}

Write a program to find average of n numbers
#include<stdio.h>
int main()
{
int n,i,sum=0,number;
float average;
printf(“Enter the number of terms”);
scanf("%d",&n);
printf(“Enter the terms”);
for(i=0;i<n;i++)
{
scanf("%d",&number);
sum=sum+number;
}
printf(“sum of numbers is %d”,sum);
average=sum/n;
printf(“average of numbers is %f”,n,average);
return(0);
}

Write a program to print weekdaysinclude<stdio.h>
int main()
{
int days;
printf(“Enter the no. of days”);
scanf("%d",&days);
switch(days)
{
case 1:printf(“monday”);
break;
case 2:printf(“Tuesday”);
break;
case 3:printf(“wednesday”);
break;
case 4:printf(“thursday”);
break;
case 5:printf(“friday”);
break;
case 6:printf(“saturday”);
break;
case 7:printf(“sunday”);
break;
default :printf(“wrong input”);
break;
}
return(0);
}

Write a program to find whether a number is odd or even#include<stdio.h>
int main()
{
int n;
printf(“Enter any number”,n);
scanf("%d",&n);
if(n%2==0)
printf(“number is even”);
else
printf(“number is odd”);
return(0);
}

Write a program to print tableinclude<stdio.h>
int main()
{
int i,mul,n,s;
printf(“Enter the number”);
scanf("%d",&n);
for(i=0;i<=10;i++)
{
mul=ni;
s=n(10+i);
printf("\n%d*%d=%d %d*%d=%d",n,i,mul,n,10+i,s);
}
return(0);
}

Write a program to check whether the number is armstrong number or not#include<stdio.h>
#include<math.h>
int main()
{
int num,sum=0,n,r;
printf(“Enter the number”);
scanf("%d",&num);
n=num;
while(n>0)
{
r=n%10;
sum= sum +(rrr);
n=n/10;
}
if(sum==num)
printf("\n %d is an armstrong number",num);
else
printf("%d is not an armstrong number",num);
return(0);
}
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(x,y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int a,int b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",a,b);
temp=a;
a=b;
b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",a,b);
}
OUTPUT:
Enter value for x:45
Enter value for y:56
Before calling swap functin
Value of x=45,Value of y=56
Inside the function
Value of a=45,Value of b=56 before swaping
Value of a=56,Value of b=45 after swaping
After returning from swap function
Value of x=45,value of y=56

Program to swap two numbers by call by reference
void swap(int *,int *);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(&x,&y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int *a,int *b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",*a,*b);
temp=*a;
*a=*b;
*b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",*a,*b);
}
OUTPUT:
Enter value for x:23
Enter value for y:45
Before calling swap functin
Value of x=23,Value of y=45
Inside the function
Value of a=23,Value of b=45 before swaping
Value of a=45,Value of b=23 after swaping
After returning from swap function
Value of x=45,value of y=23

Write a program to print details of employees
#include<stdio.h>
#include<string.h>
struct employee
{
int code;
char name[25];
char department[25];
float salary;
};
void main()
{
struct employee aemployee;
printf(“Enter employee’s code”);
scanf("%d",&aemployee.code);
printf(“Enter employee’s name”);
scanf("%s",aemployee.name);
printf(“Enter employee’s department”);
scanf("%s",aemployee.department);
printf(“Enter employee’s salary”);
scanf("%f",&aemployee.salary);
printf(“particulars of employee are “);
printf(”%d%s%s%f”,aemployee.code,aemployee.name,aemployee.department,aemployee.salary);
}
