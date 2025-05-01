# API Checklist

## Purpose:
To ensure that REST API endpoints are stable, secure, and functionally correct across different scenarios.

---

### 🔹 General
- [ ] All documented endpoints are accessible
- [ ] Endpoints return appropriate HTTP status codes (200, 201, 400, 401, 404, 500, etc.)
- [ ] Response time is acceptable (typically < 1–2 seconds)
- [ ] Endpoints handle unexpected input gracefully (e.g., missing/extra fields)

### 🔹 Authentication & Security
- [ ] Protected endpoints require authentication (401 Unauthorized if missing)
- [ ] Auth tokens expire correctly and are refreshed as expected
- [ ] Access control is enforced by user role/permissions
- [ ] Rate limiting and throttling are applied (if applicable)

### 🔹 Request Validation
- [ ] Required fields trigger validation errors when missing
- [ ] Field types are enforced (e.g., string vs. number)
- [ ] Max/min length, format, and pattern constraints are validated
- [ ] Invalid methods (e.g., PUT instead of POST) return 405 Method Not Allowed

### 🔹 Response Validation
- [ ] Response body matches expected schema (keys, data types, structure)
- [ ] No sensitive data is exposed (e.g., passwords, tokens)
- [ ] Field names are consistent and use expected naming conventions
- [ ] Pagination and sorting parameters work correctly (if implemented)

### 🔹 Error Handling
- [ ] Error messages are clear and descriptive
- [ ] Server errors (500+) are logged and do not expose stack traces
- [ ] Standardized error response format is used across endpoints

### 🔹 Data Integrity
- [ ] Data saved through POST/PUT is accurately stored in the database
- [ ] Duplicate records are not created without intention
- [ ] DELETE operations actually remove or soft-delete records as intended

---

✅ Use this checklist to verify REST API quality during development, regression testing, or backend changes.
