# Deployment notes (Cheaks68 fork)

This fork is deployed to Cloudflare Workers via Workers Builds (auto-deploy on push to main).

Worker: motion-mcp-server. Secrets MOTION_API_KEY and MOTION_MCP_SECRET live only in Cloudflare (Worker > Settings > Variables and secrets). Never commit secrets here.

To update from upstream: GitHub > Sync fork > Update branch. Cloudflare rebuilds automatically.

Fork-only changes: fast-uri lockfile security bump; MOTION_MCP_TOOLS = "complete" in wrangler.toml; this file.
