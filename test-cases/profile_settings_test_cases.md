# Test Cases – Profile Settings

## Purpose:
To validate that users can update their account settings successfully.

| ID      | Title                             | Steps                                                               | Expected Result                              | Priority |
|---------|-----------------------------------|---------------------------------------------------------------------|----------------------------------------------|----------|
| TC-101  | Change email with valid address   | Navigate to profile → Edit email → Save                             | Email is updated, confirmation sent          | High     |
| TC-102  | Change password (correct current) | Enter current password → new password → Confirm → Save              | Password is updated                          | High     |
| TC-103  | Change password (wrong current)   | Enter wrong current password → Save                                 | Error: "Incorrect current password"          | Medium   |
| TC-104  | Update display name               | Edit name field → Save                                              | Name updated in profile and UI               | Medium   |
| TC-105  | Invalid data in fields            | Enter emoji/special chars in name                                   | Error: "Invalid characters"                  | Low      |
