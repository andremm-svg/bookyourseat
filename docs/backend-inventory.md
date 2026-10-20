# Backend source inventory

A sanitized backend source archive has been prepared locally for review, but the full source has not yet been committed to this repository.

## Reviewed archive

- 71 Java source and test files
- Spring Boot / Maven project (`pom.xml`, Maven wrapper)
- PostgreSQL configuration using environment variables
- Authentication, reservations, rooms, invitations and AI assistant controllers
- 6 files under test directories

## Security review

The main application properties file references `DB_USERNAME`, `DB_PASSWORD`, `JWT_SECRET`, `SPRING_MAIL_USERNAME` and `SPRING_MAIL_PASSWORD` as environment variables. This is not a guarantee that all application secrets have been identified. Credentials previously committed or used in shared environments should be rotated.

## Release checklist

- [ ] Confirm permission to publish employer/team source code
- [ ] Review all source files and history for sensitive data
- [ ] Rotate any exposed credentials
- [ ] Verify Maven build and tests
- [ ] Add reviewed backend source
- [ ] Add and test the frontend source
- [ ] Document deployment and screenshots

Do not treat this repository as a complete or verified deployment yet.
