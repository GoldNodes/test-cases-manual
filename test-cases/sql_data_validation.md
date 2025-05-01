# SQL Data Validation Scenarios

## Purpose:
To ensure backend data matches UI expectations and system behavior.

| ID     | Scenario                                | SQL Query or Logic                                                   | Expected Outcome                            | Priority |
|--------|------------------------------------------|-----------------------------------------------------------------------|---------------------------------------------|----------|
| SQL-01 | Order created after checkout             | `SELECT * FROM orders WHERE user_id = X ORDER BY created_at DESC;`   | New record appears within expected time     | High     |
| SQL-02 | Email is stored after registration       | `SELECT email FROM users WHERE email = 'test@mail.com';`             | Email is present and unique                 | High     |
| SQL-03 | Deleted user no longer present           | `SELECT * FROM users WHERE id = 999;`                                | No result (0 rows)                          | Medium   |
| SQL-04 | Product stock decreases after purchase   | Check inventory count before and after placing an order              | Count decreases by quantity purchased       | High     |
