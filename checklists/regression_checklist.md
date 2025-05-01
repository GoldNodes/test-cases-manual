# Regression Test Checklist

## Purpose:
To ensure that existing, previously working functionality remains stable and unaffected after new changes, bug fixes, or releases.

---

### 🔹 Authentication & Authorization
- [ ] User can log in and log out
- [ ] Invalid credentials are rejected with correct error
- [ ] Password recovery and reset flows work
- [ ] Role-based access and permissions behave correctly

### 🔹 User Account & Profile
- [ ] Account registration works
- [ ] Profile update (name, email, password) works
- [ ] Email validation and uniqueness enforced

### 🔹 Core Application Flows
- [ ] Create, edit, and delete entities (e.g. orders, tasks, products)
- [ ] Forms validate input and show proper error messages
- [ ] Data is saved and persists across sessions

### 🔹 UI & Navigation
- [ ] All major pages load correctly
- [ ] Navigation between key areas works without errors
- [ ] Layout, spacing, and styles have not regressed

### 🔹 API & Backend
- [ ] Key API endpoints return expected results (200 OK, 400, etc.)
- [ ] New changes haven't broken previous response formats
- [ ] Data consistency maintained between frontend and backend

### 🔹 Payments (if applicable)
- [ ] Successful and failed payment flows function correctly
- [ ] Discounts, coupons, or promo codes are applied properly
- [ ] Confirmation messages and receipts are generated

### 🔹 Analytics & Reporting
- [ ] Dashboard data is up-to-date and correct
- [ ] Filters and date range selectors work
- [ ] Export and download functions produce accurate files

### 🔹 Notifications (Email, Push, In-app)
- [ ] Triggered notifications appear when expected
- [ ] Email templates render properly
- [ ] Unsubscribed users do not receive alerts

### 🔹 Known Bug Re-check
- [ ] Retest all fixed critical/high-priority bugs
- [ ] Check surrounding areas for regression side effects

---

✅ Use this checklist before every major release or after significant changes to ensure product stability.
