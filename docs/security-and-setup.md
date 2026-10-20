# Backend security and local setup

The original team backend archive contains environment-specific settings, including a database password and JWT secret in `src/main/resources/application.properties`. These values have intentionally not been uploaded here.

Before publishing source code:
- Replace hardcoded database credentials, JWT secrets and mail credentials with environment variables.
- Review development configuration, seed data, API examples and Postman files for sensitive values.
- Rotate any credentials that were used outside a local test environment.
- Review ownership and permission to share all team code.
- Confirm a clean checkout builds and tests successfully.

A sample `.env.example` is included at the repository root. It contains placeholders only and is not a working deployment configuration.

The source archive provided for review contains the Spring Boot backend only. Frontend source code was not included in the uploaded materials, so no runnable frontend has been published.

## QA
The supplied team test report covers 33 frontend, backend and direct API test cases. Test cases were created for UI and functional scenarios, but this repository does not claim a new successful test run.
