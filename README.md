# MoveoLoginPage

## Description
The project is about building a login and profile pages for of a website.

## Database Content
### Users info:
* guy.binyamin@gmail.com		password: a1233456
* tal@gmail.com				password: tal12346
* idan@gmail.com				password: idan123
* sapir@gmail.com				password: sapsap1
* valeryh@gmail.com			password: val1234

## Login Page
* The login page have a place to enter email and password for connecting.
* After pressing the login button it checks for valid email(by regexp) and password(6 chars with a number and a letter),
* After the page connects to the FirebaseAuth to verify that the email exists and the user entered the correct password. 
* If the email or password is not valid error massage pops up. 
* If the email dosent exists or the password is not correct error massage pops up.
* After entering the right information the user being directed to the profile page.

## Profile Page
The main perpuse of the profile page is to show all the information in the database of the user.
It shows the email, password, name, birthdate and address.
The user can change the name, birthdate and address fildes, after changing the information and pressing save the data will change in the database.
Pressing the logout button will direct the user back to the login page for reconnecting.

## Authentication
The way that the login page is authenticat the email and password is by sending them to the FirebaseAuth.
The login page will resive back if the information exists or not and if the information is correct.