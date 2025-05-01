# Test Cases – Login Functionality

## Purpose:
To verify that the login feature works correctly under normal, edge, and error conditions.

| ID      | Title                            | Steps                                                                 | Expected Result                          | Priority |
|---------|----------------------------------|-----------------------------------------------------------------------|------------------------------------------|----------|
| TC-001  | Login with valid credentials     | 1. Go to login page <br> 2. Enter valid email and password <br> 3. Click "Login" | User is redirected to dashboard | High     |
| TC-002  | Login with invalid password      | Enter valid email, wrong password → click "Login"                     | Error message: "Invalid credentials"      | High     |
| TC-003  | Empty email and password fields  | Click "Login" without entering anything                               | Validation errors shown                   | Medium   |
| TC-004  | Email format validation          | Enter "test@com" as email, valid password                             | Error: "Invalid email format"             | Medium   |
| TC-005  | Login with deactivated account   | Use credentials of deactivated user                                   | Error: "Account inactive"                 | Low      |
