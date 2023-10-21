#include <stdio.h>
#include<math.h>
int main() 
{
char op;
float a,b,result;
printf("Enter your opreator : ");
scanf("%c", &op);
printf("Enter value of a = ");
scanf("%f", &a);
printf("Enter value of b = ");
scanf("%f", &b);
switch (op)
{
    case '+': result = a+b;
    break;
    case '-': result = a-b;
    break;
    case '*': result = a*b;
    break;
    case '/': if(b!=0)
    {
        result=a/b;
    }
    else
    {
        printf("Divison not possible");
        exit(0);
    }
    break;
    default : printf("invalid opreator");
    exit(0);
    }
printf("result = %f",result);
return 0;
}
