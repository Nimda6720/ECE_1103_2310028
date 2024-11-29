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
```
#include<stdio.h>
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

-----------------------------------------------------
## **Experiment No : 02**

## **Experiment Name : Guess the Secret Number with LimitedAttempts
 Create a number guessing game where the program selects a random secret number
 between 1 and 50. The user has to guess the number, and they get unlimited attempts until
 they guess correctly. However, if they exceed 10 attempts, the game stops, and a message
 indicates that they’ve run out of attempts.
 Use a while loop to keep asking the user for guesses, and use break when:
 1.The user guesses correctly.
 2.The attempt limit (10 guesses) is reached**

## **Submission Date : 6th November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the Mathmeatical Operation :** Basically making a guessing system.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```
#include<stdio.h>
int main()
{
    printf("Welcome to the guessing game\n");
    printf("You will have 10 attempts\n");
    printf("Select a random number between \"1-50\" :\t");
    int number,i=0,s=45;
    int comparison;
    while(i<10)
    {
        i++;
        scanf("%d",&number);
        if (number>s)
        {
            comparison =1;
        }
        else if (number<s)
        {
            comparison =2;
        }
        else if  (number=s)
        {
            comparison =3;
        }
       switch (comparison) //just wanted to practice switch. That's why I used it here.
       {
       case 1:
        printf("Try lower\n");
        break;
       case 2:
       printf("Try Higher\n");
       break;
       case 3:
       printf("\"You are goddamn right\"- Walter White AKA Heisenberg\n");
       return 0;
       default:
       printf("Try something between \'1-50\'");
        break;
       }
    if (i>=10)
        {
            printf("You have ran out of attempts");
        }
    }
    return 0;
}


```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/nDGcxfT"><img src="https://i.ibb.co.com/7GfWsVH/sdsaf.png" alt="sdsaf" border="0"></a>
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/j8XwpqY/Screenshot-2024-11-06-184638.png" alt="Screenshot-2024-11-06-184638" border="0"></a>
</p>
----------------------------


## **Experiment No : 03**

## **Experiment Name : Check if an array has number 2 in it or not**

## **Submission Date : 17th November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the Mathmeatical Operation :** Just checking is an array has "2" in it or not.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```
#include<stdio.h>
int main()
{
    int array [8];
    for(int i=1; i<8; i++)
    {
        printf("Enter your %d value\t",i);
        scanf("%d", &array[i]);
    }
    for (int j=1; j<sizeof(array)/sizeof(array[0]); ++j)
    {
        if(array[j]== 2)
        {
            printf("Number 2 is found");
            break;
        }
        else
        {
            continue;
        }
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/W6zh9Pr/image.png" alt="image" border="0"></a>
</p>

-----------------------------------


## **Experiment No : 04**

## **Experiment Name : <a href="https://ibb.co.com/PZz18dT"><img src="https://i.ibb.co.com/WWpB1LD/image.png" alt="image" border="0"></a>**

## **Submission Date : 29th November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the Mathmeatical Operation :** Growth rate= principical*(1+rate/100)^years.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```
#include<stdio.h>
#include<math.h>
int main()
{
    int rate,years;
    double inv=100.0;
    printf("Enter the interest rate: ");
    scanf("%d",&rate);
    printf("Enter number of years: ");
    scanf("%d",&years);

    printf("\nYears");
    for (int i = rate; i < rate + 5; i++)
    {
        printf("\t%d%%", i);
    }
    printf("\n");

    for (int i=1; i<=years; i++)
    {
       printf("%d",i);
       for( int j=rate; j<rate+5; j++)
       {
        double amount= inv * pow(1+ j/100.0,i);
        printf("\t%.2lf",amount);
       }
       printf("\n");
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/mCmyMLf/image.png" alt="image" border="0"></a>
</p>
