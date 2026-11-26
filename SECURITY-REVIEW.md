# Security Review - Photography Studio Management System

## 1. User Roles and Access Levels

### Admin
- Full access to the system
- Manage users
- Manage customers
- Manage reservations
- Manage payments and deposits

### Manager
- Manage customers
- Manage reservations
- View payments and deposits
- Cannot manage system users

### Member
- View and create their own reservations
- View their own information
- Cannot manage users or other customers

---

## 2. Sensitive Endpoints

The following endpoints are sensitive and should require authentication and authorization:

- /users
- /customers
- /reservations
- /payments
- /admin

Access to these endpoints should be limited according to the user's role.

---

## 3. Five Security Risks

### Risk 1 - Unauthorized Access

An unauthorized user may access protected information.

Solution:
Use authentication and role-based authorization.

---

### Risk 2 - Weak Passwords

Users may use weak passwords that can be easily guessed.

Solution:
Use strong password rules and password hashing.

---

### Risk 3 - Exposed Secrets

API keys, database passwords, or secret keys may be exposed in the source code.

Solution:
Store secrets in Environment Variables and never commit them to GitHub.

---

### Risk 4 - Insecure HTTP Connection

User information may be exposed if the application uses an insecure connection.

Solution:
Use HTTPS and TLS to protect communication between the user and server.

---

### Risk 5 - Invalid User Input

Attackers may send invalid or malicious input to the application.

Solution:
Validate and sanitize all user inputs on the server side.

---

## 4. Security Recommendations

- Use Authentication and Authorization.
- Use role-based access control.
- Protect sensitive endpoints.
- Hash passwords before storing them.
- Store secrets in Environment Variables.
- Use HTTPS in production.
- Validate user input.
