#include<stdio.h>
#define KEY "Enter the calculator Operation you want to do:"
// Function prototype declaration
void addition();
void subtraction();
void multiplication();
void division();
void square();
 
// Start of Main Program
int main()
{
    char Calc_oprn;

    while(1)
    {
        printf("\n enter the operation needed");
      printf("%s : ", KEY);
 
        Calc_oprn=getche(); 
        switch(Calc_oprn)
        {
            case '+': addition();
                      break;
 
            case '-': subtraction();
                      break;
 
            case '*': multiplication();
                      break;
 
            case '/': division();
                      break;
            case '^':square();
                      break;
        }
    }
}
//addition method
void addition()
{
    int variable1,variable2, result;
    printf("\nPlease enter first number  : ");
    scanf("%d",&variable1);
    printf("Please enter second number : ");
   scanf("%d",&variable2);
   result=variable1+variable2;
    printf("Sum of entered numbers = %d \n",result);
}
 //subtraction method
void subtraction()
{ 
    int variable1, variable2, result = 0; 
    printf("\nPlease enter first number  : "); 
    scanf("%d", &variable1); 
    printf("Please enter second number : "); 
    scanf("%d", &variable2); 
    result = variable1 - variable2; 
    printf("\nsubtraction of entered numbers = %d\n", result); 
}
 
void multiplication()
{
    int variable1, variable2, result=0; 
    printf("\nPlease enter first numb   : "); 
    scanf("%d", &variable1); 
    printf("Please enter second number: "); 
    scanf("%d", &variable2);
    result=variable1*variable2;
    printf("\nMultiplication of entered numbers = %d\n",result);
}
 
void division()
{
    int variable1, variable2, result=0; 
    printf("\nPlease enter first number  : "); 
    scanf("%d", &variable1); 
    printf("Please enter second number : "); 
    scanf("%d", &variable2);
    result=variable1/variable2;
    printf("\nDivision of entered numbers=%d\n",result);
}
//square method
void square(){
    int number,result;
    printf("\nPlease enter  number  : "); 
    scanf("%d", &number); 
    result=number*number;
    printf("\nsqured number =%d",result);
}
