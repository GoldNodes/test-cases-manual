# Test Cases – API User Management

## Purpose:
To validate the functionality of REST API endpoints responsible for user management operations (CRUD).

| ID      | Title                               | Method | Endpoint            | Request Data / Params                            | Expected Result                              | Priority |
|---------|-------------------------------------|--------|---------------------|--------------------------------------------------|----------------------------------------------|----------|
| API-001 | Create user with valid data         | POST   | /api/users          | `{ "name": "John", "email": "john@test.com", "password": "Qwerty123" }` | 201 Created, returns user object or ID       | High     |
| API-002 | Create user with missing email      | POST   | /api/users          | `{ "name": "John", "password": "Qwerty123" }`    | 400 Bad Request, error: "Email is required"   | High     |
| API-003 | Get existing user by ID             | GET    | /api/users/123      | —                                                | 200 OK, returns user data                    | High     |
| API-004 | Get non-existing user               | GET    | /api/users/9999     | —                                                | 404 Not Found                                 | Medium   |
| API-005 | Update user profile                 | PUT    | /api/users/123      | `{ "name": "John Updated" }`                     | 200 OK, user data updated                     | Medium   |
| API-006 | Delete user                         | DELETE | /api/users/123      | —                                                | 204 No Content                                | Medium   |
| API-007 | Create user with existing email     | POST   | /api/users          | `{ "email": "john@test.com", ... }`              | 409 Conflict, "Email already in use"          | Medium   |
| API-008 | Unauthorized request (no token)     | GET    | /api/users/123      | — (no Authorization header)                     | 401 Unauthorized                              | High     |
