# F1 Monza Token System
This application can be used by attendees of the Monza 2022 Italian Grand Prix. All food & drink needs to be purchased using tokens. This application allows attendees to create an account and add tokens to the account which they can they use at the track to purchase food & drink.

# **User Experience & Functionality**

# User Stories
* As a first time user, I want to create an account.
* As a first time user, I want to add tokens to my account.
* As a first time user, I want to withdraw tokens from my account.
* As a first time user, I want to transfer tokens to my friend.
* As a first time user, I want to search for my friend on the system.
* As a first time user, I want to view other attendees using the system.

## Diagrams
Use Case Diagram & Class Diagram developed using [Lucid Chart](https://lucid.app/lucidchart/ae7a1d80-d51b-4265-8c00-f8b68836fd6e/edit?beaconFlowId=C5E6AF6BD782FA24&invitationId=inv_38752bd1-bdde-4c7f-8d8d-eba843da0469&page=0_0#)

![image](https://user-images.githubusercontent.com/83119583/190186382-ef471d0b-9346-41c2-a67d-67e62e8f1a7b.png)

![image](https://user-images.githubusercontent.com/83119583/190193272-6e2637eb-d03e-45dd-99eb-7ec7142cb6d2.png)

# **Features**

## Main Menu
* When the application loads successfully, a main menu is displayed with a list of options that the user to select from.
* The applications title has a pink colour to distinguish it from the menu options.
* The menu options are displayed in a liit format with a number correspoding each action.
* There is an input prompt that prompts the user to enter their selection from the menu.

![image](https://user-images.githubusercontent.com/83119583/192308716-930949a8-1487-4efe-b577-64b3bcfc28b5.png)


## View Users
* Users can view other atteendees of the grand prix who are using this system.
* Menu option '1' must be selected to open the view users dialog.
* All users of the system are displayed, the information provided is: account number, first name, last name, seat number, overdraft status & token balance.
* The column headings have a blue text colour to highlight that they are headings not user details.
* The user must click the return button to return to the main menu screen

> User Story: As a first time user, I want to view other attendees using the system.

![image](https://user-images.githubusercontent.com/83119583/192310364-308b0a09-49ba-43fc-985b-b1f70438f3a6.png)

## Add User
* New users can be added to the system, so they can avail of the token system at the Monza Grand Prix.
* Menu option '2' must be selected to open the 'add user' dialog.
* The new user will be prompted to enter their first name, last name, seat number & will have the option to sign up to an overdraft facility.
* A new users balance by default is 20 tokens.
* If a user signs up to the overdraft facility, there default balance will be 10 tokens as there is an additional charge to avail of the overdraft facility.
* If user inputs are valid, the new user is added to the system.

> User Story: As a first time user, I want to create an account.

![image](https://user-images.githubusercontent.com/83119583/192322493-28004c72-ebfd-4a12-9dee-ab642b5c1a06.png)

## Deposit Tokens
* Users can add tokens to their account, which they can use to buy food & drink around the track.
* Menu option '3' must be selected to open the 'add tokens' dialog.
* The user will be prompted to enter their account number & the amount of tokens they want to deposit.
* If user inputs are valid, the tokens will be added to their account & their balance will be updated.

> User Story: As a first time user, I want to add tokens to my account.

![image](https://user-images.githubusercontent.com/83119583/192313863-308d46cc-57be-4cf5-b990-dcd348954ede.png)

## Withdraw Tokens
* Users can withdraw tokens from their account, which they can use to buy food & drink around the track.
* Menu option '4' must be selected to open the 'withdraw tokens' dialog.
* The user will be prompted to enter their account number & the amount of tokens they want to withdraw.
* Users can withdraw an amount greater than their current balance if they are signed up to the overdraft facility.
* If the user inputs are valid, the tokens will be withdrawn from their account & their balance will be updated.
* The user will be provided with a code that they can enter at the kiosks located around the track to claim their tokens.

> User Story: As a first time user, I want to withdraw tokens from my account.

![image](https://user-images.githubusercontent.com/83119583/192315324-1244999e-f742-4360-8664-d8a9c1da92c3.png)

## Transfer Tokens
* Users can transfer tokens from one account to another, which they can use to buy food & drink around the track.
* Menu option '5' must be selected to open the 'transfer tokens' dialog.
* The user will be prompted to enter their account number & the amount of tokens they want to transfer.
* Users can transfer an amount greater than their current balance if they are signed up to the overdraft facility.
* The user will then be prompted to enter the account number of the user they want to transfer their tokens to.
* If the user inputs are valid, the tokens will be transferred from one account to another & the token balances will be updated.

> User Story: As a first time user, I want to transfer tokens to my friend.

![image](https://user-images.githubusercontent.com/83119583/192317363-1749a3fb-1d11-42b6-8c04-649e1dcea4ae.png)

## Search for User
* Users can search for other users in the system via their account number.
* Menu option '6' must be selected to open the 'search user' dialog.
* The user will be prompted to enter the account number of the user they want to find in the system.
* If the account number is valid, the searched users details will be displayed.

> User Story: As a first time user, I want to search for my friend on the system.

![image](https://user-images.githubusercontent.com/83119583/192318994-7fa789e5-63d5-49e0-b036-c48632e6d89c.png)

# Design
## Program Flow
For the design, I wanted the system to be easy to use & understand. That is why I added red text for error messages & green text for successful actions. User input is always required before the main menu screen is returned to keep the display clean & user dependent. I clear the terminal when a different menu option is selected to keep the output looking simple & less messy. 

## OOP Programming Paradigm
Object-Oriented Programming has many advantages, one of the main advantages is code reuse. Once code is written for a class, such as a user class. This code can be used re-used anytime an application needs to create a user. Inheritance works well for reusability. If you need the same functionality in multiple classes you can use a common (base) class for the same functionality and inherit that class via subclasses.
OOP results in better applications being developed, developers create highly detailed programs that are easier to maintain and update. OOP code is easier to read due to its class structure. Programs that follow another programming paradigm, such as procedural programming tend to be quite large and difficult to follow.

# Testing

## Validator Testing
I have used the PEP8 Linter to validate my code. It is activated within my visual studio. Throughout development I have been making tweaks to my code to ensure there are no errors.
View the documentation [here](https://peps.python.org/pep-0008/)

## Manual Testing
| Feature                 | Expect                                                 | Action             | Result            |
| -------------           | -------------                                          | ------------------ | -------           |
| View Users           | list of all the current users in the users.txt file should be displayed  | "User enters option "1" from the main menu. Clicks return| All users in the system are displayed|
| Add user - overdraft 'yes' | adds new user to the system with details user provided. New users balance should be 10  | "User enters option "2" from the main menu. Clicks return. Enter First Name - Lewis. Enter Last Name - Hamilton. Enters Seat Number - 5. Chooses Overdraft Facility - y. Clicks Return| User is successfully added to the system. |
| Add user - overdraft 'no' | adds new user to the system with details user provided. New users balance should be 20  | User enters option "2" from the main menu. Clicks return. Enter First Name - Fernando. Enter Last Name - Alonso. Enters Seat Number - 7. Chooses Overdraft Facility - n. Clicks Return| User is successfully added to the system. |
| Add user - first name field blank | user should not be added to the system as first name field is left blank  | User enters option "2" from the main menu. Clicks return. Enter First Name - "". Enter Last Name - Derby. Enters Seat Number - 12. Chooses Overdraft Facility - n. Clicks Return| Error message displayed informing user fields cannot be left blank |
| Add user - last name field blank | user should not be added to the system as last name field is left blank  | User enters option "2" from the main menu. Clicks return. Enter First Name - Paul. Enter Last Name - "". Enters Seat Number - 3. Chooses Overdraft Facility - n. Clicks Return| Error message displayed informing user fields cannot be left blank |
| Add user - seat number field blank | user should not be added to the system as seat number field is left blank  | User enters option "2" from the main menu. Clicks return. Enter First Name - Paul. Enter Last Name - Richards. Enters Seat Number - "". Chooses Overdraft Facility - n. Clicks Return| Error message displayed informing user fields cannot be left blank |
| Add user - overdraft field blank | user should not be added to the system as overdraft field is left blank  | User enters option "2" from the main menu. Clicks return. Enter First Name - Mary. Enter Last Name - Evans. Enters Seat Number - 47. Chooses Overdraft Facility - "". Clicks Return| Error message displayed informing user there is an invalid overdraft input |
| Add user - overdraft field number | user should not be added to the system as overdraft field has invalid integer input  | User enters option "2" from the main menu. Clicks return. Enter First Name - Mary. Enter Last Name - Evans. Enters Seat Number - 47. Chooses Overdraft Facility - 2. Clicks Return| Error message displayed informing user there is an invalid overdraft input |
| Add user - overdraft field letter | user should not be added to the system as overdraft field has invalid input  | User enters option "2" from the main menu. Clicks return. Enter First Name - Mary. Enter Last Name - Evans. Enters Seat Number - 47. Chooses Overdraft Facility - ddeeg. Clicks Return| Error message displayed informing user there is an invalid overdraft input |
| Deposit Tokens| user balance is updated based on number of tokens added | User enters option "3" from the main menu. Clicks return. Enter Account Number - 0. Clicks Return. Tokens to deposit - 10. Click Return| Tokens are added to users balance & successful message is displayed |
| Deposit Tokens - invalid account number| user balance should not be updated as invalid account number has been entered | User enters option "3" from the main menu. Clicks return. Enter Account Number - 7. Clicks Return. Tokens to deposit - 10. Click Return| Error message displayed informing user that account number cannot be found |
| Deposit Tokens - invalid account number| user balance should not be updated as invalid account number has been entered | User enters option "3" from the main menu. Clicks return. Enter Account Number - h. Clicks Return. Tokens to deposit - 10. Click Return| Error message displayed informing user that the account number is invalid & are prompted to enter another account number |
| Deposit Tokens - string token amount| user balance should not be updated as invalid token amount has been entered| User enters option "3" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return. Tokens to deposit - ten. Click Return| Error message displayed informing user that the token amount must be a whole number |
| Deposit Tokens - 0 token amount| user balance should not be updated as invalid token amount has been entered| User enters option "3" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return. Tokens to deposit - 0. Click Return| Error message displayed informing user that deposit amount cannot be 0 |
| Deposit Tokens - empty token amount| user balance should not be updated as invalid token amount has been entered| User enters option "3" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return. Tokens to deposit - "". Click Return| Error message displayed informing user that the token amount must be a whole number |
| Withdraw Tokens| user balance is updated based on number of tokens withdrawn | User enters option "4" from the main menu. Clicks return. Enter Account Number - 0. Clicks Return. Tokens to withdraw - 3. Click Return| Tokens are withdrawn from users balance & successful message is displayed |
| Withdraw Tokens - no overdraft| user balance should not be updated as they are trying to withdraw an amount greater than their balance & are not signed up to the overdraft facility. | User enters option "4" from the main menu. Clicks return. Enter Account Number - 0. Clicks Return. Tokens to withdraw - 10. Click Return| Error messaged displayed informing the user they have insufficient funds & that they are not signed up to the overdraft facility |
| Withdraw Tokens - overdraft| user balance is updated based on number of tokens withdrawn | User enters option "4" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return. Tokens to withdraw - 30. Click Return| Tokens are withdrawn from users balance & successful message is displayed |
| Withdraw Tokens - invalid account number| user balance should not be updated as invalid account number has been entered  | User enters option "4" from the main menu. Clicks return. Enter Account Number - 27. Clicks Return. Tokens to withdraw - 30. Click Return| Error message informing the user that the account number cannot be found  |
| Withdraw Tokens - invalid account number| user balance should not be updated as invalid account number has been entered  | User enters option "4" from the main menu. Clicks return. Enter Account Number - h. Clicks Return. Tokens to withdraw - 30. Click Return| Error message displayed informing user that the account number is invalid & are prompted to enter another account number |
| Withdraw Tokens - string token amount| user balance should not be updated as invalid token amount has been entered| User enters option "4" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return. Tokens to withdraw - twenty. Click Return| Error message displayed informing user that the token amount must be a whole number |
| Withdraw Tokens - token amount 0 | user balance should not be updated as invalid token amount has been entered| User enters option "4" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return. Tokens to withdraw - 0. Click Return| Error message displayed informing user that the token amount must be greater than 0 |
| Search User | searched users details should be displayed | User enters option "6" from the main menu. Clicks return. Enter Account Number - 1. Clicks Return.| User found successfully & information is displayed |
| Search User - invalid account number | user should be informed that account number is invalid | User enters option "6" from the main menu. Clicks return. Enter Account Number - 27. Clicks Return.| Error message displayed informing user account number cannot be found|
| Search User - invalid account number string | user should be informed that account number is invalid | User enters option "6" from the main menu. Clicks return. Enter Account Number - 'account number 4'. Clicks Return.| Error message displayed informing user account numbers is invalid|
| Transfer Tokens | tokens transferred from one account to another & both balances are updated | User enters option "5" from the main menu. Clicks return. Enter Account Number - '0'. Clicks Return. Tokens to transfer: 3. Click Return. Account number to transfer: 1. Click Return| Message informing the user that the tokens have been transferred sucessfully & both users balances are updated|
| Transfer Tokens - no overdraft | tokens should not be transferred as user is trying to transfer tokens greater than their current balance & are not signed up to the overdraft facility | User enters option "5" from the main menu. Clicks return. Enter Account Number - '0'. Clicks Return. Tokens to transfer: 10. Click Return. Account number to transfer: 1. Click Return|  Error message informing the user that they have insufficient funds & are not signed up to the overdraft facility|
| Transfer Tokens - overdraft | tokens transferred from one account to another & both balances are updated | User enters option "5" from the main menu. Clicks return. Enter Account Number - '1'. Clicks Return. Tokens to transfer: 40. Click Return. Account number to transfer: 0. Click Return| Message informing the user that the tokens have been transferred sucessfully & both users balances are updated|
| Transfer Tokens - same account number | tokens should not be transferred as user is trying to transfer tokens to the same account number | User enters option "5" from the main menu. Clicks return. Enter Account Number - '0'. Clicks Return. Tokens to transfer: 10. Click Return. Account number to transfer: 0. Click Return|  Error message informing the user that they cannot transfer funds to the same account number|
| Transfer Tokens - invalid transfer account number | tokens should not be transferred as user is trying to transfer tokens to the same account number | User enters option "5" from the main menu. Clicks return. Enter Account Number - '0'. Clicks Return. Tokens to transfer: 10. Click Return. Account number to transfer: 27. Click Return|  bug - no error message displayed|
| Invalid Menu Option | no function should be called as the user input is invalid | User enters option "10" from the main menu.|  Error message informing user choice is invalid|
| Invalid Menu Option - string | no function should be called as the user input is invalid | User enters option "m" from the main menu.|  Error message informing user choice is invalid|
| Exit System | system should stop running, no further inputs can be accepted| User enters option "7" from the main menu.|  system no longer running, no inputs accepted|

## Bugs Identified During Development & Testing
* When I first began creating my file structure & variable names, I was using the camel case naming convention. I was not aware that it was best practise to use the snake case naming convention when creating variables in python. I updated my variables & used snake case throughout the rest of my project.
* In my datastore class, I did not create a users property, so when I was trying to call the users property in menu.py I was getting an error that the list could not be found. I then created the users property in the datastore class so I could access the users within the menu.
* In my user class, I created the balance variable as a string & when I tried to perform any arithmetic operations such as add and substract, I was getting an error that a string and int cannot concatenate. I converted the balance parameter to an int within the user class to fix this bug.
* When I completed writing an if else statement, I did not unindent my code & was writing code within the else block. I unindented my code to fix this issue.
* In the overdraft validation, I was using 'or' instead of 'and' in my if statement. Using 'or' meant that only one conditional needed to be met while an 'and' statement means both conditionals need to be met.
* Within my while loops, I was using JavaScript syntax of '==' instead of 'is', which is the correct approach in Python. I was also adding redundant brackets to my if statements & while loops.
* When I called view users function, the data was only visible if I scrolled up in the terminal as the menu was being displayed after the function call. I added an input("return to continue") to the function so the menu would only return when the user was done reading the user list.
* When I was calling my functions, I forgot to add the 'self.' keyword at times.
* When validating the account number in the search function, I originally called a NameError however this accepted string inputs so I updated it to a ValueError.
* When trying to use the built in 'cls' function in the OS module, I got an error saying 'cls' was not recognised. After some research I found a solution where I had to alternatively use 'clear'.
* I needed to add some comments to my commits as my commit messages did not explain all the code written.
* No error message is displayed when the account number that is receiving transferred tokens is invalid.
* Seat number can only be numbers, not accepting strings.
* When adding a user, first name is accepting special characters such as '@;0#@' etc.
* Some of my commit messages have spelling errors, however this is due to an issue with the bash terminal. I type the commit message correctly however it is changed after I confirm the commit.
![image](https://user-images.githubusercontent.com/83119583/192360064-9b54a089-e789-43ad-9774-1b5fd64e2066.png)







