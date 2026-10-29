# Agent Running house rules

- This is not a blindness, disability or CharliVerse site. Keep it separate from Blind Ant, Carrados and charli.info.
- Follow `brand/brand-book.md` and `brand/tokens.json` exactly: Agent Running wordmark in international orange, navy P.S. mark as the only icon, archival cream and charcoal grounds, Libre Caslon Display / Source Serif 4 / IBM Plex Mono.
- No Golden Gate Bridge, robots, circuit boards or generated images. Illustrations, if any, are code-drawn SVG.
- Write as Piper, in the first person, British spelling, short operational sentences, each rule ending on one line that sticks.
- Piper's public biography is "Cambridge, Navy, civil service". Never name an intelligence service.
- Every page carries the disclosure in its footer and its meta description: Piper Smith is a fictional author created by Charli-Jo Tyrer; the operations, ideas and evidence are real.
- One H1 per page. Build to ZIC: contrast checked in light and dark, real text not images of text, each rule a heading.
- Publishing is Cloudflare Workers Builds from GitHub (since 29 October 2026), the same as Charli.info: merging to `main` of `Carrados/AgentRunning` publishes. The trigger "agent-running production" runs `node scripts/build-worker.mjs` then `npx wrangler deploy`, and watches `site/`, `scripts/`, `worker.js` and `wrangler.toml`.
- To change the site: edit `site/index.html` on a `claude/<topic>` branch, run `node scripts/build-worker.mjs` so `worker.js` in the repo matches, open a pull request to `main`, and merge once Charli-Jo approves. Check the build afterwards (Workers & Pages, `agent-running`, Deployments) or ask Claude to read it through the Cloudflare connector.
- Never upload `worker.js` by hand through the API or paste pages into the dashboard: that would overwrite what Workers Builds deployed from `main`. Keep it as an emergency fallback only, and say so before using it.
- `wrangler.toml` keeps `workers_dev` and `preview_urls` off, so the site is only at its own domain.
- The Worker serves agentrunning.uk and www.agentrunning.uk (www redirects to the bare domain) as Workers custom domains.
- The domain's email stays with IONOS. Never touch its MX, SPF, DKIM, DMARC, autodiscover or domainconnect records.
