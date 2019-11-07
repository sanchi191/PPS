Write a program to print calculatorvoid main()
{
        int num1, num2, res;
        char op;
        printf("Enter the First number");
        scanf("%d", &num1);
        printf("Enter the second number");
        scanf("%d", &num2);
        printf("What operation do you want to perform /
        /s for sum, b for subtract, d for divide , m for multiply ");
        scanf(" %c",&op);

switch(op)
{
        case 's':
                res = num1 + num2;
                printf("The sum of the chosen number is %d", res );
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
The product of the chosen number is :1035

Write a program for bubble sorting
