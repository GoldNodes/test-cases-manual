# Test Cases – Notifications and Alerts

## Purpose:
To ensure proper behavior of user notifications and system alerts.

| ID      | Title                             | Steps                                                               | Expected Result                              | Priority |
|---------|-----------------------------------|---------------------------------------------------------------------|----------------------------------------------|----------|
| TC-201  | Receive email after registration  | Complete signup process                                             | Welcome email is delivered                   | High     |
| TC-202  | Push notification on new message  | Receive message in-app (with push enabled)                          | Device gets notification                     | High     |
| TC-203  | Disable email notifications       | Go to settings → turn off email alerts                              | User no longer receives notification emails  | Medium   |
| TC-204  | Alert for failed payment          | Simulate failed payment in checkout                                 | Error alert shown + email sent               | High     |
| TC-205  | Language of notifications         | Change app language → trigger alert                                 | Message appears in selected language         | Medium   |
