----------
## **Experiment No : 01**

## **Experiment Name : Create a simple banking system in C using a switch statement to manage these menu 
options:
 1.Deposit: Ask for an amount and add it to the balance.
 2.Withdraw: Ask for an amount and deduct it if funds are sufficient; otherwise, show an 
error.
 3.Balance Inquiry: Display the current balance.
 4.Exit: End the program.
 Validate inputs to prevent negative deposits or withdrawals and handle insufficient funds**

## **Submission Date : 5th November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the Mathmeatical Operation :** Basically making a simple bank management system.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```#include<stdio.h>
int main()
{
float amount,balance=6456.00;
int choice;
while (1)
 {
    printf("\n Make a choice:");
    printf("\n1.Deposit");
    printf("\n2.Withdraw");
    printf("\n3.Balance Inquiry");
    printf("\n4.exit");
    printf("\nEnter your choice\n");
    scanf("%d", &choice);
 switch (choice)
  {
 case 1:
    
    printf("Enter the amount that you want to add\n");
    scanf("%f", &amount);
    if (amount<=0)
    {
        printf("Add a positive number\n");

    }
    else
    {
        balance+=amount;
        printf("Your current balance is%f\n",balance);
    }
    break;
 case 2:
   printf("Enter the amount of money you want to withdraw\n");
   scanf("%f", &amount);
   if (amount>balance)
   {
    printf("You can't print the money that you don't have");
   }   
   else
   {
    balance-=amount;
    printf("You now have\t %f",balance);
   }
   break;
 case 3:
   printf("Your Balance is %.2f/n",balance);  
   break;
 case 4:
     printf("Exiting the program");
     return 0; 
 
 default:
    break;
  }


return 0;
 }
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/pXSXy4W/Screenshot-2024-11-05-235914.png" alt="Screenshot-2024-11-05-235914" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>image uploader</a><br />
  <a href="https://imgbb.com/"><img src="https://i.ibb.co.com/9sx083f/Screenshot-2024-11-06-000021.png" alt="Screenshot-2024-11-06-000021" border="0"></a>
  <a href="https://imgbb.com/"><img src="https://i.ibb.co.com/c2qn3jy/Screenshot-2024-11-06-000217.png" alt="Screenshot-2024-11-06-000217" border="0"></a>
</p>

