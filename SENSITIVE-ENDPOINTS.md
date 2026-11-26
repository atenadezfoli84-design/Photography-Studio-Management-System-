# Sensitive Endpoints

The following endpoints contain sensitive information and require authentication and authorization.

| Endpoint | Access |
|---|---|
| /users | Admin |
| /customers | Admin, Manager |
| /reservations | Admin, Manager, Member |
| /payments | Admin, Manager |
| /admin | Admin |

Access to each endpoint should be controlled according to the user's role.
