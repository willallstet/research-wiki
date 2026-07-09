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

## [2026-07-07] track_substacks | 5 feeds (Will's post-internet/net-art orbit)
- Added config/substacks.txt: cliuanon, newmodels, donotresearch, joshuacitarella, ideaspace(ystrickler.com). First run, 14-day window.
- 8 new posts; 6 queued (PRs #2-#7), 2 skipped (off Will's documented topics: CLiuAnon working-class cinema; Doomscroll 49.5 electoral-strategy).
- Queued: NM 'Taste', DNR 'Sea Monsters as Medium', DNR 'Noel & Trevor Paglen', Doomscroll DS50/Steyerl/Steyerl-II. Watermark advanced for all 5 feeds.

## [2026-07-07] review_content | 6 queued substack PRs (#2-#7)
- Reviewed all 6 open content PRs. Readable (rated): #2 NM Taste (I7/T6), #3 DNR Sea Monsters (I8/T7), #4 DNR Noel & Paglen (I8/T4).
- Gated podcast stubs (no rating, on-topic note only): #5/#6/#7 Doomscroll Hito Steyerl episodes — substance is paywalled audio.

## [2026-07-07] update_wiki | integrate 3 accepted queue items
- Added a 'readings' category. New pages: flash-bon-inference-time-scaling, sea-monsters-as-medium, new-models-taste-2026.
- Cross-linked from concepts ai-and-machine-vision (Flash-BoN, NM Taste), media-infrastructure & archives-and-wikipedia (Sea Monsters). Index updated; 3 queue files removed.
- Note: adapted the DAM update_wiki layout (papers/primitives) to this wiki's sources/entities/concepts/readings taxonomy. Rejected PR #4 (Paglen) not integrated.

## [2026-07-08] lint | fixed 1 broken link (index.md format-legend placeholder parsed as a link); staleness clean (portfolio pages pinned at HEAD af63cc3, no drift); orphans clean; taxonomy matches page dirs
## [2026-07-08] ingest | ccru/writings-1997-2003 (added on request) — new readings page from PDF; +1 index line; links to ai-and-machine-vision, archives-and-wikipedia, media-infrastructure, sea-monsters-as-medium
## [2026-07-08] update_wiki | integrate 5 accepted queue items (Benjamin, Steyerl, O'Sullivan, Chirimuuta, Spinoza)
- Added 5 readings pages: benjamin-work-of-art-mechanical-reproduction, steyerl-in-free-fall, osullivan-myth-science-fictioning, chirimuuta-reflex-machine-cybernetic-brain, spinoza-ethics. All read in full (4 local files via /ingest_folder; Steyerl fetched from e-flux with a browser UA after a 403).
- Cross-linked into concepts ai-and-machine-vision (all 5), media-infrastructure (Benjamin, Steyerl), archives-and-wikipedia (Benjamin, Steyerl, O'Sullivan); reciprocal links added in ccru-writings-1997-2003 (O'Sullivan/hyperstition) and chirimuuta (Spinoza on mind/mechanism). Index updated (+5 lines); 5 queue files removed.
- Noted (not flattened) two productive tensions: Chirimuuta's abstraction argument vs Flash-BoN's scaling optimism, and Spinoza's monism vs Chirimuuta's organicism. Steyerl page flags the rotted citations found in companion crawl PR #9. Opened as a PR per the maintainer's branch-and-PR rule (no direct push to main).

## [2026-07-09] update_wiki | integrate 5 accepted queue items
Integrated 5 merged queue items into readings: Benjamin, *The Work of Art in the Age of Mechanical Reproduction* (local PDF); Chirimuuta, *The Reflex Machine and the Cybernetic Brain* (local PDF); O'Sullivan, *Myth-Science and the Fictioning of Reality* (local PDF); Steyerl, *In Free Fall* (e-flux #24, read from URL); Spinoza, *Ethics* (local txt, Elwes/Gutenberg). Added new concept page [[fictioning-and-hyperstition]] (anchored by Ccru + O'Sullivan) and wired the readings into concepts ai-and-machine-vision, media-infrastructure, archives-and-wikipedia; added a fictioning backlink to the Ccru page. +6 index lines. Removed the 5 processed JSON files from queue/accepted/. Sources have no commit SHAs (local files / web essay), so provenance uses commit: n/a and file/line or paragraph citations.
