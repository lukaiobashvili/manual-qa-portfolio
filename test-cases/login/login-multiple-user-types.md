Module: Login 
App: SauceDemo (saucedemo.com) 
Tester: Luka Iobashvili
Date: 22.09.2026

This file covers login behavior across all standard SauceDemo test accounts. Each row is treated as its own test case since the same steps are run with different input data (the username), a common pattern called data-driven testing.

-----------------------------------------------------------------------------------------------------------------------------------------------------

Test_ID: TC-001
Title: Verify that standard_user can log in to the account
Preconditions: User has a registered account and is on the login page
Priority: High

Steps: 	
1. Navigate to the saucedemo.com login page
2. Enter username: standard_user
3. Enter the password: secret_sauce
4. Click the "Login" button
5. Observe the product listing page

Expected Result: User logs in successfully and sees the product listing page with all product images displaying correctly
Actual Result: User logs in successfully and sees the product listing page with all product images displaying correctly
Status: Pass

-----------------------------------------------------------------------------------------------------------------------------------------------------

Test_ID: TC-002
Title: Verify locked_out_user can't log in to the account
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






