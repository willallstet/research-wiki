# Wiki log

Chronological, append-only log of what happened and when. Newest entry last.
Entry format:

`## [YYYY-MM-DD] <onboard|ingest|lint|query> | <subject>`

## [2026-07-07] onboard | initialise: Will Allstetter personal-site + research-interests wiki
- Purpose, taxonomy (sources/entities/concepts), source, remote, and weekly cron (Mon 07:23) written to wiki.config.json.
- THIS-WIKI.md specialised for the personal-site domain; maintenance schedule sched-c95a20ffe760 created.

## [2026-07-07] ingest | willallstet/simple2026portfolio @af63cc3
- First (tiered eager) pass. Added 1 source page, 4 entity pages (will-allstetter, affiliations, published-writing, art-projects), 3 concept pages (ai-and-machine-vision, archives-and-wikipedia, media-infrastructure).
- Watermark advanced to af63cc3a3b2137db130fafb4bc8ada75257de74a.
- Flagged for lint: several untitled embedded videos in index.html (YouTube/Vimeo) need names.

## [2026-07-07] scan_arxiv | willallstet/research-wiki keywords
- Scanned 25 arXiv keywords (from Will's crawled interest profile) over a 2-day window (2026-07-05..07).
- 23/25 keywords completed; 2 unresolved after retries due to arXiv HTTP 429 (content-based image retrieval, multimodal embeddings) — coverage gap noted.
- 1 candidate found, 1 queued: PR #1 arXiv 2607.04461 Flash-BoN (text-to-image inference-time scaling).
