# Upstream notes

This package is intentionally bounded to a single Cosmos-native application contribution.

Before upstream submission:

1. Install it on a clean Cosmos host and retain the streamed creation log.
2. Confirm the generator and configuration containers exit successfully.
3. Confirm PostgreSQL and Synapse become healthy and the bootstrap container exits successfully.
4. Log in with a Matrix client using the selected Cosmos hostname.
5. Verify `/_matrix/client/versions`, `/_matrix/federation/v1/version`, `/.well-known/matrix/client`, and `/.well-known/matrix/server` through the public Cosmos route.
6. Restart the entire stack and confirm the immutable identity and administrator markers are reused.
7. Restore a coordinated Synapse-data/PostgreSQL backup and repeat the checks.
8. Decide whether to retain the neutral SVG icon or replace it with an upstream-approved Synapse mark.
