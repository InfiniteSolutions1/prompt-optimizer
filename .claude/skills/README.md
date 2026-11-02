# Social media scraping setup

Two tools for reading Instagram, YouTube, TikTok and other social posts from Claude Code.

## 1. Apify MCP server (`.mcp.json`)
Official server from https://github.com/apify/apify-mcp-server at `https://mcp.apify.com`.
Claude can search Apify Store and run scrapers (Actors) such as Instagram post/reel scrapers.

- Needs env var: `APIFY_TOKEN` (from https://console.apify.com/settings/integrations)
- Needs network access to: `mcp.apify.com`, `api.apify.com`
- Paid per run on Apify (free tier available)

## 2. ScrapeCreators skills (this folder)
Copied from https://github.com/ScrapeCreators/social-media-research-skills (MIT, commit 64ba7b4).
`scrapecreators-api` is the core skill; the others are research workflows built on it.

- Needs env var: `SCRAPECREATORS_API_KEY` (from https://scrapecreators.com)
- Needs network access to: `api.scrapecreators.com`

## Cloud environment setup
Add the env vars and allowed domains above in the cloud environment settings
(environment menu in the session title bar -> Edit), then start a new session.
Never commit the keys to this repo.
