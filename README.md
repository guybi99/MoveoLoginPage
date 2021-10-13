# MoveoLoginPage

## Description
The project is about building a login and profile pages for a website.

## Database Content
### Users info:
* guy.binyamin@gmail.com		password: a1233456
* tal@gmail.com				password: tal12346
* idan@gmail.com				password: idan123
* sapir@gmail.com				password: sapsap1
* valeryh@gmail.com			password: val1234

## Login Page
* The login page has a place to enter an email address and a password for connecting.
* After pressing the login button it checks for a valid email (by regexp) and password (6 chars with a number and a letter).
* Then, the page connects to the FirebaseAuth to verify that the email exists and that the user has entered the correct password. 
* If the email or password is not valid, an error message pops up. 
* If the email dosen't exists or if the password is not correct, an error message pops up.
* After entering the right information, the user is directed to the profile page.

## Profile Page
The main purpose of the profile page is to show all the information in the database of the user.
It shows the email, password, name, birthdate and address.
The user can change the name, birthdate and address fields. After changing the information and pressing save the data will change in the database.
Pressing the logout button will direct the user back to the login page for reconnecting.

## Authentication
The way that the login page  authenticates the email and password is by sending them to the FirebaseAuth.
The login page will recieve back if the information exists or not and if the information is correct.
