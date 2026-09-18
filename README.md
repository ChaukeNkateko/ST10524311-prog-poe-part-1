# ST10524311-prog-poe-part-1

This is a simple but robust Java console application I built to handle user account creation, validation and login. The whole idea was to make sure it follows strict programming rules and uses automated testing to catch errors.
#What the project does

The program runs in the console and gives the user a clean experience to enter their registration details. It checks the formatting rules straight away as the user types and then later verifies the login details against what was registered.
#Username Check:#

The username has to contain an underscore (_) and it can't be longer than 5 characters.If it doesn't meet this, the program tells the user and asks agaim
Password Complexity: I made sure the password is actually secure. It has to be at least 8 characters long and must have at least one uppercase letter, one number, and one special character.
Cell Phone Number Check: This checks if the phone number is in the correct international format. It validates the structure so that only properly formatted numbers are accepted.2. 
Login AuthenticationOnce the user has registered, the login part compares what they enter during login with the details that were stored in memory. Depending on whether it matches or not, it shows a custom message to let the user know if login was successful or failed.
I used Apache NetBeans 20, but any version should workTo run
:Open the project in NetBeans.Find PROGPOE.java in the Projects panel on the left.
Right click on it and click Run File, or just press Shift + F6
.Then you can test it in the output terminal — try entering both correct and wrong details to see the validation working.
TestingI used JUnit  for testing. 
The tests cover the main edge cases:testRegisterUser() 
checks if a valid registration workstestInvalidUsername()
makes sure wrong usernames are caughttestInvalidPassword() 
checks that weak passwords are blockedtestReturnLoginStatus() -
tests if the login messages are correctTo run the tests, right click on the project folder and click Test, or press Alt + F6. If everything is green, all tests passed
