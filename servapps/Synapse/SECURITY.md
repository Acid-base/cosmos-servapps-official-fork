# Security boundary

The Matrix client and federation protocol route must remain directly reachable and therefore must not be placed behind Cosmos browser authentication, SmartShield challenges, or bot filtering. Synapse's admin API is not separately routed by this package. The registration shared secret remains inside the generated homeserver configuration volume. Database and Synapse application secrets are retained through Cosmos-managed environment and volume state.
