# CI/CD Pipeline

## Pipeline Flow

GitHub Push
↓
Build
↓
Test
↓
Test Passed?
↓
Deploy
↓
Production

## Test Failure

If a test fails, the pipeline stops and the application is not deployed.

Build → Test → Failed → Stop

If all tests pass:

Build → Test → Passed → Deploy → Production
