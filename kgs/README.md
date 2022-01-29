# Key Generation Service (KGS)

## Requirements

-   Install [Wrangler](https://github.com/cloudflare/wrangler#installation) CLI for Cloudflare Workers deployment.
-   Install [Miniflare](https://miniflare.dev/cli.html) CLI for local development work.

## Installation

```sh
npm ci
```

## Development

To test out the cron trigger locally, run the following:

```sh
# At terminal 1
miniflare

# At terminal 2
curl "http://localhost:8787/.mf/scheduled"
```

Note that no actual keys will be created on your actual Cloudflare KV namespaces (not even `preview`). By default, KV data is stored in memory.

## References

-   https://miniflare.dev/storage/kv