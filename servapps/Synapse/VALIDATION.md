# Validation

The service graph was checked against the current Cosmos `ContainerCreateRequestContainer` JSON surface and against Cosmos command tokenization (`strings.Fields`).

Executable checks cover:

- generator first run and idempotent rerun;
- yq configuration with passwords containing shell punctuation and spaces;
- PostgreSQL projection;
- reverse-proxy-aware listener configuration;
- Matrix well-known projection;
- closed public registration;
- immutable `server_name` refusal;
- runtime refusal before configuration closure;
- runtime refusal after identity drift;
- private PostgreSQL networking;
- Cosmos-owned ingress without a host port;
- SmartShield and bot filtering disabled on the Matrix protocol route.

A real Cosmos fresh-install, restart, upgrade, federation, and backup/restore pass remains required before proposing this package upstream.
