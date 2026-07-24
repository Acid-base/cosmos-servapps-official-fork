# Matrix Synapse for Cosmos

The hostname selected in Cosmos becomes Synapse `server_name` and is permanent. Changing it after first installation is intentionally refused.

The package converges through idempotent generator, configuration, runtime, and administrator-bootstrap containers. Cosmos owns the secure proxy network and routes both Matrix client and federation traffic directly to port 8008. SmartShield and browser authentication are intentionally disabled for the protocol route.

Back up the Synapse data volume and PostgreSQL volume as one consistency unit. A TURN service is still required for reliable voice and video calls.
