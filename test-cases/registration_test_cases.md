# Test Cases – Registration Flow

## Purpose:
To verify that the user registration form functions properly under various conditions.

| ID      | Title                                | Steps                                                                 | Expected Result                              | Priority |
|---------|--------------------------------------|-----------------------------------------------------------------------|----------------------------------------------|----------|
| TC-001  | Register with valid data             | Fill in all fields → Submit                                          | Success message and user account created     | High     |
| TC-002  | Register with existing email         | Use email already in use → Submit                                    | Error: "Email already registered"            | High     |
| TC-003  | Password and confirm mismatch        | Enter different passwords → Submit                                   | Error: "Passwords do not match"              | Medium   |
| TC-004  | Missing required fields              | Leave name/email empty → Submit                                      | Field-level validation errors                 | Medium   |
| TC-005  | Invalid email format                 | Enter "test@com" → Submit                                            | Error: "Invalid email format"                | Medium   |
| TC-006  | Weak password                        | Use short/simple password → Submit                                   | Error: "Password too weak"                   | Low      |
