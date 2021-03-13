# Homework 5: Chapter 4

## 4.5: Using the technique suggested here, where natural language descriptions are presented in a standard format, write plausible user requirements for the following functions: 

**An unattended petrol (gas) pump system that includes a credit card reader. The customer swipes the card through the reader, then specifies the amount of fuel required. The fuel is delivered and the customer's account is debited.**

   1.1 The system shall read and authenticate a customer's credit card. (This will require the customer to swipe card and enter zip code)

   1.2 The system shall output transaction details, via a screen.

   1.3 The system shall allow a customer to input the desired amount of gas.

   1.4 The system shall deliver gas to the customer's vehicle. (This can only be done after 1.1, 1.2 and 1.3 have completed)

   1.5 The system shall charge the customer's card.

   1.6 The system should print a reciept.

   1.7 The system should clear information about the customer's transaction once the transaction is complete.


**The cash-dispensing function in a bank ATM**

   1.1 The system shall accept the customer's ATM card or debit card

   1.2 The system shall accept the customer's PIN through a numpad entry

   1.3 The system shall authenticate card and PIN with records at their bank

   1.4 The system shall allow the customer to diplay balance amounts.

   1.5 The system shall accurately dispense money, in $20 increments, when the customer makes a withdrawal.

   1.6 The system shall update the bank's balance records to reflect the transaction

   1.7 The system shall delete all records of the transaction details once it confirms the bank has the updated account details 


**In an Internet banking system, a facility that allows customers to transfer funds from one account held with the bank to another account with the same bank.**

   1.1 The system shall allow the customer to login to their account with a username and password through a webpage or portal

   1.2 The system should provide the customer with the ability to reset their password. (This should be handled with current password entry and a second form of authentication, such as an email, text, or phone notification.)

   1.3 The system shall retrieve the customer's account details.

   1.4 The system shall allow the customer to select the origination and destination accounts for the transfer

   1.5 The system shall allow the customer to input a transfer amount, only allowing valid amounts. (Non-negative, less than or equal to current balance, etc)

   1.7 The system should move the specified amount from the origination account to the destination amount. (after all above requirements are met)

   1.8 The system should output a confirmation of the transaction

   1.9 The system should redirect to the accounts page


## 4.6: Suggest how an engineer responsible for drawing up a system requirements specification might keep track of the relationships between functional and non-functional requirements.
 
   "you should, ideally, highlight requirements that are clearly related to emergent system properties...by putting them in a separate section of the requirements document or by distinguishing them in some way from other system requirements." - Sommerville

   This means engineers should seperate functional requirements from the non-functional with having seperate lists altogether or by constructing a heirachy of requirements to highlight the importance of some that put them at a higher priority.

## 4.7: Using your knowledge of how an ATM is used, develop a set of use cases that could serve as a basis for understanding the requirements for an ATM system.

**USECASE 1: Check account balance**

   The customer walks up to the ATM and inserts their card (bank/ATM/debit). The system then prompts for the PIN that corresponds to the card, which the customer then enters via a numpad or touch interface. The ATM then processes the info and authorises the customer, displaying options (Withdrawal, Check Balance, Transfer). The customer then selects the Check Balance. The ATM then displays account details (current balance, ledger balance, etc). The system then prompts the customer if they want a receipt. Once the customer inputs their choice, the ATM returns to the main screen with the options.

**USECASE 2: Withdrawal**

   The customer walks up to the ATM and inserts their card (bank/ATM/debit). The system then prompts for the PIN that corresponds to the card, which the customer then enters via a numpad or touch interface. The ATM then processes the info and authorises the customer, displaying options (Withdrawal, Check Balance, Transfer). The customer then selects the Withdrawal option. The ATM then displays a prompt for the customer to select an account to withdraw from. The customer selects the account they want to withdraw from. The ATM then prompts for the withdrawal amount. The customer then enters the amount. After checking the validity of the amount entered, the ATM processes the withdrawal and dispenses the amount requested in $20 bills. The system then prompts the customer if they want a receipt. Once the customer inputs their choice, the ATM returns to the main screen with the options.












