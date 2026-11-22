# Poker Fate Stats

Poker Fate Stats was a searchable archive of Texas Hold'em player profiles from Poker Fate. The site displayed each profile's collection time and used separate tags for preflop and postflop play in six-max Hold'em.

Collection stopped on 2026-09-03 when guest login began returning device verification error `-5`. The production and preview sites are offline. The [login findings](docs/research/api-inventory.md#login-rejection-and-recovery) document what changed.

- [Web app](web/README.md) for local development and tests.
- [Python tools](python/README.md) for the collector and D1 import from saved snapshots.
- [Research notes](docs/research/README.md) on player discovery, the tagging model, and the client API.
