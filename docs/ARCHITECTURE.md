# Architecture overview

VESTDRAC is intended to provide one shared virtual execution environment for multiple independent strategy instances.

1. **Market observations:** labeled historical fixtures and controlled read-only market observations.
2. **Signal evaluation:** per-strategy conditions and temporal validation.
3. **Virtual execution:** isolated simulated orders, positions, fees, limits and results.
4. **Recovery:** checkpoints and repeatable offline verification in supported paths.
5. **Presentation:** sanitized result data for separately managed interfaces.

The architecture separates virtual fills from broker executions and test fixtures from historical observations. No source code, detailed algorithms or private schemas are published. Public market-feed readiness and full strategy parity are not claimed.
