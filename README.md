#include<stdio.h>
#include<string.h>
#include<stdlib.h>


double price[7] = {15.80 , 10.50 , 19.00 , 14.00 , 12.00 , 22.00 , 16.00 };
double mealTaxPrices[7];
int adultNumber,childNumber;


void printMeals();
void orderMeals();
double orderForAdult();
double orderForChildren();
int main()
{
    char response = 'y';
    
     
     printMeals();
     while(response == 'y'|| response == 'Y')
    {
            printf("please enter number of adults  :");
            scanf("%d",&adultNumber);
            
            printf("please enter number of children:");
            scanf("%d",&childNumber);
            
                       
            orderMeals();
            
            printf("\nwould you like to continue(y/n):");
            scanf("\n%c",&response);
    }
  
 printf("\n      *** THANK YOU FOR COMING  ****\n");
 printf("\20****   PLEASE VISIT US NEXT TIME  ****\20 \n");
   system("pause");
   return 0;
}

void printMeals()
{
     
      printf("\20***  WELCOME TO BVPS RESTURANT ****\20\n");
      printf(" \t\t\t Below is the menue:\20\n");
      printf(" \t\t\t MEALS\t\t\tPRICE:\n");
      printf(" \t\t\t \22*****\22\n");
      printf(" \t\t\t 1- Chips\tRS15.80\n");
      printf(" \t\t\t 2- Noodles\tRS10.50\n");
      printf(" \t\t\t 3- Fried Rice\tRS19.00\n");
      printf(" \t\t\t 4- Chicken Chop\tRS14.00\n");
      printf(" \t\t\t 5- Chicken Soup\tRS12.00\n");
      printf(" \t\t\t 6- Corn Soup\tRS22.00\n");
      printf(" \t\t\t 7- Seafood Platter\tRS16.00\n");
