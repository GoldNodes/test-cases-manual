# Smoke Test Checklist

## Purpose:
To quickly verify that the core functionality of the application works and that the build is stable enough for further testing.

### 🔹 Authentication
- [ ] Login with valid credentials
- [ ] Logout functionality
- [ ] Prevent login with invalid credentials

### 🔹 Main Navigation
- [ ] Dashboard/homepage loads successfully
- [ ] Navigation menu links are clickable and lead to correct pages
- [ ] User can navigate between key sections without errors

### 🔹 Core Features
- [ ] User can create a new record (e.g., order, item, task)
- [ ] User can edit an existing record
- [ ] User can delete a record and receive confirmation
- [ ] Search or filter returns results (if applicable)

### 🔹 UI & Stability
- [ ] No broken images or missing styles
- [ ] No critical JavaScript errors in console
- [ ] Page reload works without crashing
- [ ] Application loads under normal conditions without timeouts

### 🔹 API & Backend
- [ ] API `/status` or health check returns 200 OK
- [ ] Application connects to database and returns data
- [ ] No visible backend errors (500, 502, 503)

### 🔹 Environment
- [ ] Correct version number is visible (if applicable)
- [ ] Environment variables/settings are correct for build (e.g., staging, production)
