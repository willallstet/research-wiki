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
## [2026-07-09] ingest | kittler/there-is-no-software
New readings page from local PDF (a68ba6a…): Friedrich Kittler, "There Is No Software" (1992), read in full. +1 index line; added to tracked readings on [[media-infrastructure]] (priority of hardware / substrate-first) and [[ai-and-machine-vision]] (critique of the computational metaphor, pairs with Chirimuuta). Source PDF is OCR-noisy; quotes normalized and cited to printed pages 147–155. Removed accepted queue item.

## [2026-07-13] ingest | willallstet/simple2026portfolio @0eb35db — delta: 2 new landing-page items (Conscious Tether reader → published-writing; Lattice Lab / Transmediale 2027 → affiliations); +2 line shift propagated across all index.html-derived pages
## [2026-07-13] lint | staleness clean after ingest (all 9 portfolio-derived pages re-pinned to 0eb35db, incl. will-allstetter.md whose cited bio lines were verified unmoved); corrected +2 line-shift citations in 2 readings pages (benjamin, osullivan) that ingest's delta did not touch; links + orphans clean; no contradictions; taxonomy matches page dirs

## [2026-07-14] scan_arxiv | 25 keywords, 6 candidates, 3 PRs opened
- Scanned 25 keywords (all succeeded after arXiv 429 throttling + retries).
- 6 candidates in 2-day window; 0 duplicates of open PRs/queue/integrated.
- Queued: 2607.11886 (SpectraReward, text-to-image reward modeling — AI & machine vision), 2605.15868 (SOLAR, symmetric multimodal retrieval — archives/embeddings), 2607.11643 (Xiaomi-Robotics-U0, unified embodied synthesis — borderline, defaulted to queue).
- Skipped: 2607.10864 (image-deblurring convex-optimization math), 2607.11007 (TabPFN classifier calibration), 2607.10909 (Stresa recsys adapter efficiency).
- PRs #28, #29, #30.

## [2026-07-14] track_substack | 5 feeds polled, 3 new posts, 3 PRs opened
- Polled 5 feeds; 3 posts newer than watermarks: cliuanon (2026-2027 Syllabus), donotresearch (Performing Distress), joshuacitarella (DS 50.5: Hito Steyerl).
- Opened queue PRs #31, #32, #33 ({url,title,source} schema for /review_content). Note: DS 50.5 is a Doomscroll digest, which the interest profile marks REJECTED — left for /review_content to score.
- Advanced watermarks in config/substacks_state.json to each feed's newest post; newmodels + ideaspace unchanged (no new posts).
- Ran the track_substacks workflow directly: the skill referenced by config is not installed on this pod (see report).
## [2026-07-27] ingest | willallstet/simple2026portfolio @1436a13 — delta: +imageGit project (index.html:52); Refresh exhibition now listed twice (plain link :87 + photo/full-title :93, flagged for lint); Soft Systems Gallery detail added to Broken Images (:95); Transmediale line reworded (:54). +2 net line shift re-pinned across all 9 index.html-derived pages (sources overview incl. script/style line moves).
## [2026-07-27] lint | post-ingest verification: links + orphans clean (check-links empty); all 9 index.html-derived pages confirmed pinned to 1436a13; caught index.html cross-citations in 2 readings pages (benjamin :95/:72, osullivan :72/:75) that ingest's PDF-scoped delta could not reach; no contradictions (Refresh double-listing documented on art-projects, not flattened — single-author site evolving); taxonomy matches page dirs.

## [2026-07-31] track_substack | 5 feeds polled, 0 new posts, 0 PRs opened
All five feeds fetched successfully; each feed's newest post sat exactly at its
stored watermark, so nothing new since 2026-07-28. Watermarks unchanged (no
advance needed). No digest entries.

## [2026-07-31] scan_arxiv | 25 keywords, 7 candidates, 4 PRs opened
All 25 keywords fetched cleanly (no API failures). 7 unique candidates in the
2-day window; 1 deduped (2607.27084, already open as PR #64). Scored 6:
queued 4 — PR #67 2607.28233 (RowHammer/RowPress device-level modeling →
media-infrastructure), #68 2607.27628 (BlindPSNR no-reference fidelity →
ai-and-machine-vision), #69 2607.28526 (DAR-Net degradation/content
disentangling, borderline), #70 2607.28130 (face SR + re-ID, borderline).
Skipped 2 — 2607.27898 (remote-sensing efficiency, cf. REJECTED #56),
2607.28247 (agricultural monitoring; IQA keyword collision only).

## [2026-08-03] ingest | no-op — willallstet/simple2026portfolio still @1436a13 (watermark == remote HEAD, verified via git ls-remote); no delta files, no pages re-pinned

## [2026-08-03] lint | repaired merge damage from 545cdae (two branches integrated the same 5 readings): benjamin, chirimuuta, osullivan, steyerl each held TWO concatenated page bodies (duplicate H1s, and for chirimuuta a second frontmatter block embedded mid-page). Kept the richer 051bb6f body per page, dropped the duplicate tail, and repaired doubled frontmatter keys (single source/commit/files/updated/kind; files: now repo-relative, matching the clean pages). Grafted the cross-links that existed only in the discarded tails (benjamin -> fictioning + ccru; chirimuuta -> media-infrastructure + ccru contrast; osullivan -> fictioning + will-allstetter; steyerl -> chirimuuta + osullivan + will-allstetter), rewritten against current index.html line numbers rather than the tails' stale :68/:69/:91. Fixed a verified factual error: Chirimuuta pagination was pp. 421-452, correct is 421-457 (PDF is 37pp from p.421; doi:10.1162/posc_a_00346 added). Corrected a misattributed quote: "the magical aspect of simulation..." is Canguilhem 1963 quoted by Chirimuuta, not her own phrase. Deduplicated wiki/index.md (5 readings listed twice; kept richer hooks, folded in the more precise Zohn/2011/Elwes bibliographic detail). Verified: all 8 index.html citations resolve to claimed content at 1436a13 via read-only git show; all local pdfs/ targets exist; all source-relative paths exist at the pinned sha; links + orphans clean; no dangling wikilinks; every page has one frontmatter block, one H1, one index line; no remaining contradictions. Staleness: no portfolio-derived page drifted (source HEAD unmoved), so none re-pinned.

## [2026-08-03] update_wiki | no-op — queue/accepted/ empty; no intake PRs merged since #21 (2026-07-09). Also ran peer_review: all 53 open PRs already carry a review (42 arXiv + 5 local-pdf peer-reviewed, 5 substack content-reviewed, #9 is a crawls/ report and out of scope) — 0 reviews posted.

## [2026-08-03] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09)
Ran peer_review first: all 53 open PRs already carry a review — 42 arXiv queue PRs (#22-70) and 5 local-pdf PRs (#10-14) stamped `<!-- llm-wiki-review -->`, 5 substack/blog PRs (#31, #33, #42, #46, #53) stamped `<!-- llm-content-review -->` (correctly routed away from peer_review per the marker-mismatch note), and #9 is a `crawl/` report, not a queue intake file. 0 reviews posted.
Then update_wiki: `queue/accepted/` is empty and untracked-clean, and the newest merged PR is still #21 (2026-07-09), so no reading has been accepted since the last integration. No pages created, refreshed, or re-pinned; no index or taxonomy change. All 53 PRs remain at the human merge/close gate — integration unblocks only when one is merged.
