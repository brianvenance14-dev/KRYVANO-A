# Architecture
- `src/server.js`: Express application entry point.
- `src/config`: environment validation and database pool.
- `src/middleware`: authentication, roles, validation, errors.
- `src/routes`: HTTP endpoints.
- `src/services`: business logic and external provider adapter.
- `src/db`: SQL migrations and migration runner.
- `public`: static responsive client.
- `uploads`: temporary local uploads only; not durable on ephemeral hosts.

All privileged decisions are enforced on the server. The browser is never trusted to assign roles or access Owner routes.
