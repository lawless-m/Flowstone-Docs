# KeycloakUpdater

A [[RocsMiddleware]] service that syncs customer contacts from PostgreSQL to [[Keycloak]] user management.

**Repo:** `~/Git/RocsMiddleware/KeycloakUpdater`
**Themes:** [[csharp]], [[dotnet]], [[Keycloak]]

Reads contacts from PostgreSQL, creates or updates Keycloak users in MySQL with permission attributes (image downloads, banned products, planogram access). Hash-based change tracking with simulation mode for testing.
