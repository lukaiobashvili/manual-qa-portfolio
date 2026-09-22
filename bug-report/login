Bug ID: BUG-001
Title: Login error message reveals - "Sorry, this user has been locked out"
Reported by: Luka Iobashvili
Date found: 22.09.2026
Environment: Chrome, MacOS device
Severity: High
Priority: High
Status: Open
Related Test Case: TC-001
Steps to Reproduce:
1. Navigate to https://www.saucedemo.com
2. Enter username locked_out_user
3. Enter password secret_sauce
4. Click "Login"
5. Observe the error message displayed

Expected Result: User can't log in and sees a generic error message "Invalid username or password"
Actual Result: User can't log in but sees "Sorry, this user has been locked out"
<Screenshot/Recording attached>

Why this matters: Per authentication guidelines, login error messages should be generic. Revealing a specific 'locked out' status confirms the account exists, enabling username enumeration
Recommendation: Use a generic error message for all login failures ("invalid username or password") so no response reveals account existence or status
