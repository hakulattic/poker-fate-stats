# Poker Fate Stats Web

The React app displays Texas Hold'em player snapshots from Cloudflare D1. The production and preview deployments are offline. The [tagging model](../docs/research/player-tagging.md) explains how the site classified players.

## Development

From the `web/` directory, start the frontend at <http://127.0.0.1:5178/>.

```bash
pnpm install
pnpm run dev
```

From the repository root, run the frontend checks and the Playwright smoke tests.

```bash
nix develop --command scripts/check-web.sh
```

The smoke tests use [sample snapshots](tests/fixtures/) and run their own server on port `5179`. The [Wrangler configuration](wrangler.toml) records the production and preview database bindings. The [preview seed](seeds/preview-players.json) contains sample players.
