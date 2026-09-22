Test_ID: TC-002
Title: Verify locked_out_user can't log in to the account
Tester: Luka Iobashvili
Date: 22.09.2026
Preconditions: User has a registered account that is locked, and the user is on the login page
Priority: High

Steps: 	
1. Navigate to the saucedemo.com login page
2. Enter username: locked_out_user
3. Enter the password: secret_sauce
4. Click the "Login" button
5. Observe the product listing page

Expected Result: The user can't log in and sees a generic error message "Invalid username or password"
Actual Result: The user can't log in and sees an error message "Sorry, the user has been locked out"
Status: Fail
Related Bug: Bug-002
