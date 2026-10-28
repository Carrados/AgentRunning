# Agent Running house rules

- This is not a blindness, disability or CharliVerse site. Keep it separate from Blind Ant, Carrados and charli.info.
- Follow `brand/brand-book.md` and `brand/tokens.json` exactly: Agent Running wordmark in international orange, navy P.S. mark as the only icon, archival cream and charcoal grounds, Libre Caslon Display / Source Serif 4 / IBM Plex Mono.
- No Golden Gate Bridge, robots, circuit boards or generated images. Illustrations, if any, are code-drawn SVG.
- Write as Piper, in the first person, British spelling, short operational sentences, each rule ending on one line that sticks.
- Piper's public biography is "Cambridge, Navy, civil service". Never name an intelligence service.
- Every page carries the disclosure in its footer and its meta description: Piper Smith is a fictional author created by Charlotte Joanne; the operations, ideas and evidence are real.
- One H1 per page. Build to ZIC: contrast checked in light and dark, real text not images of text, each rule a heading.
- Publishing: edit `site/index.html`, run `node scripts/build-worker.mjs` to regenerate `worker.js`, commit both, then upload `worker.js` to the Worker `agent-running` through the Cloudflare API. Never paste pages into the dashboard by hand.
- The Worker serves agentrunning.uk and www.agentrunning.uk (www redirects to the bare domain) as Workers custom domains.
- The domain's email stays with IONOS. Never touch its MX, SPF, DKIM, DMARC, autodiscover or domainconnect records.
