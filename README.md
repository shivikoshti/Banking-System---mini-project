# Mini-project-
## Banking Management system<br>
The code is designed to simulate a simple banking system with two types of accounts: current_account and saving_account.<br>
## Class Definitions:<br>
class account:<br>
Private Members:<br>
name: Stores the name of the account holder.<br>
accno: Stores the account number.<br>
atype: Stores the type of account (although it's never used explicitly in any logic).<br>
Public Members:<br>
getAccountDetails(): A function to input account details from the user.<br>
displayDetails(): A function to display the account holder's details.<br>
class current_account:<br>
Inheritance: This class inherits from the account class.<br>
Private Members:<br>
balance: Stores the balance of the current account.<br>
Public Members:<br>
c_display(): Displays the balance.<br>
c_deposit(): Allows the user to deposit an amount into the account.<br>
c_withdraw(): Allows the user to withdraw an amount. The withdrawal is allowed only if the balance is more than 1000.<br>
class saving_account:<br>
Inheritance: This class inherits from the account class.<br>
Private Members:<br>
sav_balance: Stores the balance of the savings account.<br>
Public Members:<br>
s_display(): Displays the balance.<br>
s_deposit(): Allows the user to deposit an amount and also adds interest to the deposited amount (2% of the balance after the deposit).<br>
s_withdraw(): Allows the user to withdraw an amount. The withdrawal is allowed only if the balance is more than 500.<br>

## Main Function:<br>
The main() function performs the following steps:<br>

It creates objects c1 for current_account and s1 for saving_account.<br>
The user is prompted to enter the type of account they want to operate (S for savings and C for current).<br>
Based on the user's choice:<br>
For saving_account:<br>
User's account details are taken.<br>
A menu-driven system is displayed to the user, allowing them to deposit, withdraw, display balance, display full details, or exit.<br>
For current_account:<br>
User's account details are taken.<br>
Similar menu-driven system as above.<br>
If the user enters a choice other than 'S', 's', 'C', or 'c', an error message is shown.<br>
The program ends by displaying a thank-you message.<br>
