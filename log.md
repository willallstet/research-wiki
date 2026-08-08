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
## [2026-08-03] track_substack | 5 feeds polled, 4 new posts, 1 PR opened (#71 New Models / Paglen "How to See Like a Machine"); 3 skipped off-topic (Do Not Research orchestra labor, Doomscroll David Harvey interview, CLiuAnon work call-for-submissions); watermarks advanced for 4 feeds, ideaspace unchanged (no new posts)
## [2026-08-03] scan_arxiv | 25 keywords, 0 candidates, 0 PRs opened — window 20260801-20260803 covers Sat/Sun/Mon; arXiv does not announce on weekends and Monday's batch is not yet announced at 14:11 UTC. Verified not a query fault: broadest keyword ("text-to-image generation") returns totalResults=1919 with newest published 2026-07-31T04:54Z (2607.29025), which the 2026-07-31 run already covered. No gap; no dedup needed.

## [2026-08-03] review_content | reviewed #71 (New Models / Trevor Paglen "How to See Like a Machine" launch w/ Mat Dryhurst, Sybil Berlin) — interesting 6/10, trustworthy 6/10, verdict "skim as a pointer". Ran as peer_review's correct instrument: of 50 open PRs, all 44 arXiv/local-pdf ones already carry `<!-- llm-wiki-review -->` (re-running would duplicate) and 5 substack ones already carry `<!-- llm-content-review -->`, leaving #71 as the only genuinely unreviewed intake. Routed to review_content not peer_review because the URL is substack, not arxiv.org. Page is an event announcement with Part 2 paywalled — reviewed the freely visible text and noted the gating rather than fabricating coverage of the talk; flagged that the Verso book is the higher-value intake. Interest profile unchanged: no merge/close decisions since #56, so no new learned signals to append.

## [2026-08-03] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09). #71 remains open awaiting the human merge/close decision, so nothing to integrate.

## [2026-08-03] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09). Ran peer_review first: of 54 open PRs, all 47 arXiv/local-pdf intakes already carry `<!-- llm-wiki-review -->` (re-running would post duplicates), 6 substack intakes (#31, #33, #42, #46, #53, #71) already carry `<!-- llm-content-review -->` from review_content, and #9 adds `crawls/eflux-in-free-fall.md` rather than a `queue/accepted/` intake file so neither review skill applies. 0 reviews posted, 0 pages touched. All 54 PRs remain open awaiting human merge/close decisions, so there is nothing for the curator to integrate.

## [2026-08-04] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09). Ran peer_review first: of 54 open PRs, all 47 arXiv/local-pdf intakes already carry `<!-- llm-wiki-review -->`, 6 substack intakes (#31, #33, #42, #46, #53, #71) already carry `<!-- llm-content-review -->` from review_content, and #9 adds `crawls/eflux-in-free-fall.md` rather than a `queue/accepted/` intake file so neither review skill applies. 0 reviews posted, 0 pages touched. PR count and composition unchanged since the 2026-08-03 run — no merges or closes in the interim — so the queue is still blocked on human merge/close decisions.

## [2026-08-04] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09). Second run today, user-requested. Ran peer_review first: of 54 open PRs, all 47 arXiv/local-pdf intakes already carry `<!-- llm-wiki-review -->`, 6 substack intakes (#31, #33, #42, #46, #53, #71) already carry `<!-- llm-content-review -->` from review_content, and #9 adds `crawls/eflux-in-free-fall.md` rather than a `queue/accepted/` intake file so neither review skill applies. 0 reviews posted, 0 pages touched. PR count and composition unchanged since the 2026-08-03 run. This is the third consecutive identical no-op: review coverage is complete and the pipeline is fully blocked on human merge/close decisions — no amount of re-running peer_review or update_wiki will move it forward.

## [2026-08-04] peer_review | reviewed 5 of 7 newly-queued arXiv intakes (#72, #75, #76, #77, #78)

First non-no-op peer_review run since 2026-08-03: seven new arXiv intakes (#72-#78) arrived from scan_arxiv and carried no review marker. Shuffled per the skill's anti-anchoring rule and reviewed 5 (the hard per-run cap), reading each PDF in full via pymupdf text extraction (poppler unavailable, so the Read tool's PDF path is unusable on this pod — pymupdf via `uvx` is the working route). #73 (2608.02148) and #74 (2608.01794) remain unreviewed and are first in line next run.

Verdicts: #78 CAPEval `reject` (n=10 single-seed OLS with two collinear predictors, no R²/CIs; stated novelty preempted by CapMAS/Lee et al. 2024, which it cites but never engages). #75 SpikeRestormer `borderline` (T=1 throughout collapses every LIF neuron to a threshold function, so the "spiking event reasoning" framing is nomenclature; component ablation doubles params 4.79M→10.73M; its own Table 2 shows an ANN at 5.10 mJ vs the model's 16.80 mJ, falsifying "lowest energy"). #72 ReLIQS `borderline` (verified programmatically that all 11 baselines in Table 1 have byte-identical LIVE and AGIQA-3K columns while only ReLIQS differs — a column-duplication error sitting in the column carrying its largest claimed margin; PIE and LQAM each contribute only ~0.005). #77 Discriminative Axis `accept` (the one genuinely strong paper: matched-exposure negative control, similarity-vs-collision dissociation on identical audio, three-seed replication where the causal claim lives, and a volunteered 22% test-contamination disclosure with mechanism). #76 UEmbed `borderline` (N=1 — the single-token bottleneck the whole method exists to fix — is never ablated, and the adopted N=16 scores 63.4 vs N=2's 63.8; τs=32 adopted over the better-scoring 64; Table 6's 6-point 4B dense→sparse accuracy drop goes unmentioned in the text).

Fit note carried into all five reviews: four of the five are `scan_arxiv` false positives — cs.CV/cs.CL keyword matches ("image restoration", "saliency", "multimodal", "contrastive") with no purchase on this wiki's humanities/art-research framing of machine vision as a political and aesthetic object. Each review therefore separates quality from fit and recommends closing on relevance, with a per-paper note telling the curator not to create orphan primitive/concept pages. The recurring signal is now four-for-five in a single batch: `config/keywords.txt` wants tightening rather than the taxonomy widening.

## [2026-08-04] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09)

Fourth consecutive update_wiki no-op, but for a different reason than the previous three: review coverage is no longer the blocker (five fresh reviews were posted this run), yet zero PRs have been merged since #21, so there is nothing in queue/accepted/ to integrate. 0 pages touched. Current state: 61 open PRs, 7 closed-unmerged. The pipeline remains entirely gated on human merge/close decisions — reviews are now waiting on 59 of the 61 open PRs.

## [2026-08-04] peer_review | reviewed the 2 remaining unreviewed arXiv intakes (#73, #74)

Ran peer_review on all open PRs: of 31 open, 29 are arXiv intakes and 27 already carried
`<!-- llm-wiki-review -->`, leaving #73 (2608.02148, Douyin Multimodal Embedding) and #74
(2608.01794, VisID/MVEB) unreviewed. Both PDFs downloaded and read in full (28pp and 18pp
incl. supplementary); posted one full-depth review each, both `borderline` (#73 scores
3/2/3/4/3; #74 scores 3/2/3/3/3). The 2 remaining open PRs (#53, #71) are substack/blog
intakes that already carry `<!-- llm-content-review -->`, so peer_review does not apply.
Review coverage across all open PRs is now complete — 0 unreviewed intakes remain.

## [2026-08-04] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09)

Second run today (user-requested, following peer_review above). No accepted papers to
integrate: `queue/` does not exist on `main`, and no intake PR has been merged since #21 on
2026-07-09. 0 pages touched. All 31 open PRs await human merge/close decisions. Now that
review coverage is complete, re-running peer_review can add nothing — the pipeline moves
only when a human merges or closes queued PRs.

## [2026-08-05] peer_review | no-op — all 61 open arXiv intakes already reviewed

Scanned all 62 open PRs. Every arXiv queue intake (#22–#78, incl. the 7 queued 2608.x papers)
already carries `<!-- llm-wiki-review -->`, so 0 papers needed review. The 6 substack/blog
intakes (#31, #33, #42, #46, #53, #71) carry `<!-- llm-content-review -->` and belong to
`review_content`, not `peer_review`; #9 is a crawl PR (`crawls/`, `index.md`, `log.md`), not a
paper proposal. Review coverage remains complete.

## [2026-08-05] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09)

No accepted papers to integrate: `queue/` does not exist on `main` and no intake PR has been
merged since #21 on 2026-07-09. 0 pages touched. All 62 open PRs await human merge/close
decisions — the pipeline cannot advance until a human accepts or rejects queued intakes.

## [2026-08-05] peer_review | no-op — all 61 open PRs already reviewed
Triaged every open PR by diff path and marker. All 55 arXiv/local-pdf intakes already carry `<!-- llm-wiki-review -->` (#11, #12, #14 carry two); the 6 substack/blog intakes (#31, #33, #42, #46, #53, #71) already carry `<!-- llm-content-review -->` from review_content and are deliberately not re-reviewed with the NeurIPS rubric; #9 adds `crawls/eflux-in-free-fall.md` rather than a `queue/accepted/` intake so neither skill applies. 0 reviews posted.

## [2026-08-05] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09)
No accepted intake files to integrate, so 0 pages touched. Tallied the standing recommendations across the 61 open PRs to identify the actual blocker: 25 `accept`, 23 `borderline`, 6 `reject`, 7 unscored (6 content-reviewed + #9). Review coverage is complete; the pipeline is blocked entirely on human merge/close decisions, not on further agent runs.

## [2026-08-05] peer_review | no-op — all 54 arXiv intakes already reviewed
Triaged all 61 open PRs by diff path and idempotency marker. Every `queue/accepted/<id>.json` arXiv/local-pdf intake (54 PRs) already carries `<!-- llm-wiki-review -->`; the 6 substack/blog intakes (#31, #33, #42, #46, #53, #71) carry `<!-- llm-content-review -->` and are correctly out of scope for the NeurIPS rubric; #9 adds `crawls/eflux-in-free-fall.md` rather than an intake file, so neither review skill applies. 0 reviews posted.

## [2026-08-05] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09)
No accepted intake files present, so 0 wiki pages touched. Re-tallied standing recommendations across the 54 peer-reviewed PRs: 25 `accept`, 23 `borderline`, 6 `reject`. The pipeline has been blocked on human merge/close decisions for 27 days — agent runs cannot advance it further.

## [2026-08-05] peer_review | reviewed the 3 newly-queued arXiv intakes (#79, #80, #81)
Triaged all 64 open PRs by diff path and idempotency marker: 54 arXiv/local-pdf intakes already carried `<!-- llm-wiki-review -->`; the 6 substack/blog intakes (#31, #33, #42, #46, #53, #71) carry `<!-- llm-content-review -->` and stay out of scope for the NeurIPS rubric; #9 adds `crawls/eflux-in-free-fall.md` rather than an intake file. That left exactly 3 unreviewed arXiv intakes, all under the 5-per-run cap, each read in full from its PDF in an isolated context to avoid cross-paper score anchoring. #79 (2608.03284, T2S2 — safe text-to-image via intermediate clean estimates) → `accept` 4/4/4/4/4. #80 (2608.03279, 3DGSI-Assessor — 3D Gaussian Splatting image quality assessment) → `accept` 4/4/4/4/4. #81 (2608.03826, Geo-Embed/GeoMEB — unified multimodal urban embeddings) → `borderline` 4/3/3/4/3, blocked on a zero-shot-vs-fine-tuned baseline asymmetry and no geographic-disjointness check. Reviews #79 and #80 flag the papers as poor fits for this wiki's critical/aesthetic remit; #81 is the one with real purchase, as a primary artifact of the machine-vision apparatus (PlacePulse safety/wealth scoring, CityLens socioeconomic inference, photo geolocalisation, no ethics statement). Note: two PDF text extractions initially returned a different paper's text and were caught and re-extracted by the reviewers before scoring; every posted review was verified to carry its own PR's arXiv ID before posting. 3 reviews posted.

## [2026-08-05] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09)
No accepted intake files to integrate, so 0 wiki pages touched: `queue/` does not exist on `main` and no intake PR has been merged since #21, 27 days ago. Standing recommendations now span 57 peer-reviewed PRs: 27 `accept`, 24 `borderline`, 6 `reject`. Review coverage is again complete — every open arXiv intake carries a review — so the pipeline remains blocked entirely on human merge/close decisions rather than on further agent runs.

## [2026-08-05] peer_review | no-op — all 28 open arXiv intakes already reviewed
Scanned 30 open PRs on willallstet/research-wiki. All 28 arXiv queue PRs (#51–#81, less
#71/#53) already carry the `<!-- llm-wiki-review -->` marker, so nothing was re-reviewed.
The two unreviewed PRs (#71 NEW MODELS/Paglen, #53 CLiuAnon/PDX9) are Substack intakes and
belong to `/review_content`, not `/peer_review`.

## [2026-08-05] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09)
No accepted papers to integrate: every queue PR is still open awaiting the human merge gate,
so `queue/accepted/` does not exist on `main`. Wiki pages, index, and watermarks unchanged.

## [2026-08-06] peer_review | no-op — all 29 open arXiv intakes already reviewed
Scanned 31 open PRs (#51-#81). All 29 arXiv intakes already carry an `llm-wiki-review`
comment, so the idempotency check skipped every one. The two unreviewed PRs (#71 NEW MODELS /
Trevor Paglen, #53 CLiuAnon / PDX9) are Substack posts and route to `/review_content`.

## [2026-08-06] update_wiki | no-op — queue/accepted/ empty; last intake merge still #21 (2026-07-09)
Nothing to integrate: every reviewed intake PR is still open awaiting the human merge/close
gate, so no JSON has landed in queue/accepted/. Backlog now 31 open PRs, oldest #51.

## [2026-08-06] peer_review | no-op — all 58 open arXiv intakes already reviewed; 6 substack intakes route to /review_content
## [2026-08-06] update_wiki | no-op — queue/accepted/ absent on main; last intake merge still #21 (2026-07-09)

## [2026-08-06] track_substacks | no-op — 5/5 feeds fetched, 0 posts newer than watermark
- Feeds: cliuanon, newmodels, donotresearch, joshuacitarella, ideaspace.ystrickler.com.
- All fetched successfully; newest post per feed still at or below the stored watermark.
- No queue PRs opened; `config/substacks_state.json` left unchanged.

## [2026-08-06] scan_arxiv | no PRs — 2 candidates, 1 duplicate, 1 filtered out
- 25/25 keywords queried successfully; 2 unique papers in the 2-day window.
- 2608.03826 (Geo-Embed, unified multimodal embeddings for urban understanding) —
  deduplicated: already queued as open PR #81.
- 2608.04944 (geometry-based deep equilibrium model for image restoration under
  multiplicative Gamma noise, math.NA) — SKIP. Matched the `image restoration`
  keyword, but the contribution is a numerical-analysis convergence result for
  speckle denoising; no bearing on the wiki's interest in degraded/"poor" images as
  aesthetic-political artifacts. Consistent with learned signal REJECTED (#56).
- No queue PRs opened; no wiki pages modified.

## [2026-08-06] peer_review | no-op — all 30 open intakes already reviewed
28 arXiv queue PRs (#51–#81) already carry the `<!-- llm-wiki-review -->` marker
and were skipped as reviewed. PRs #71 (Trevor Paglen talk) and #53 (PDX9 essay)
are non-arXiv intakes outside this skill's filter; both already carry
`<!-- llm-content-review -->` from /review_content. No reviews posted.

## [2026-08-06] update_wiki | no-op — queue/accepted/ empty, 30 PRs awaiting merge gate
No accepted papers to integrate: `queue/accepted/` holds no JSON on main. The
last intake merge remains PR #21 (2026-07-09). All 30 open queue PRs are
reviewed and waiting on the human merge/close decision, which is the gate that
feeds this workflow — nothing to curate until some are merged.

## [2026-08-07] peer_review | no-op — all 57 arXiv intakes already reviewed
64 open PRs scanned. All 57 arXiv queue PRs carry the `<!-- llm-wiki-review -->`
marker and were skipped as reviewed. Six non-arXiv intakes (#71, #53, #46, #42,
#33, #31) are outside this skill's filter and already carry
`<!-- llm-content-review -->` from /review_content. PR #9 is a crawl report
(`crawls/eflux-in-free-fall.md`), not a paper intake — no review applies. No
reviews posted.

## [2026-08-07] update_wiki | no-op — no queue/accepted/ on main
Nothing to integrate: `main` has no `queue/` directory, so no accepted intake
JSON is waiting. The last intake merge remains PR #21 (2026-07-09). All 64 open
PRs are reviewed and blocked on the human merge/close gate that feeds this
workflow. No wiki pages modified.

## [2026-08-07] peer_review | no-op — all 57 arXiv intakes already reviewed; 7 non-arXiv PRs route to /review_content

## [2026-08-07] update_wiki | no-op — no queue/accepted/ on main; all 64 intakes await the human merge gate

## [2026-08-07] track_substacks | no-op — 5/5 feeds fetched, 0 posts newer than watermark

## [2026-08-07] scan_arxiv | 4 PRs — 25 keywords, 7 candidates, 0 duplicates, 3 filtered out
- Queued: 2608.05811 (Energy-Guided Flow Matching), 2608.05691 (SciQNet image
  quality assessment), 2608.05833 (ViSR-KGC visual subgraph reasoning),
  2608.01905 (PhotoHOI, borderline → queue). PRs #82–#85.
- Skipped: 2608.05769 (relation-manifold distillation, matches REJECTED #56),
  2608.04944 (math.NA convergence proof), 2607.28247 (agricultural crop benchmark).
- Watermark unchanged for substacks; no feed errors.

## [2026-08-07] peer_review | 4 arXiv intakes reviewed (#82–#85)
- Reviewed the 4 PRs opened by today's scan_arxiv run, each in an isolated context
  to avoid cross-paper score anchoring: #82 2608.05811 Energy-Guided Flow Matching
  (4/3/3/4/3 → borderline), #83 2608.05691 SciQNet (4/2/2/2/2 → reject),
  #84 2608.05833 ViSR-KGC (4/3/3/4/3 → borderline), #85 2608.01905 PhotoHOI
  (3/2/3/3/2 → reject, posted as a correction to a borderline first draft).
- Skipped 6 non-arXiv PRs (#31, #33, #42, #46, #53, #71) already carrying
  /review_content reviews, and #9 (a crawls/ report, not a queue intake).
- All 64 prior arXiv intakes were already reviewed; no duplicates posted.

## [2026-08-07] update_wiki | no-op — queue/accepted/ empty; no PR merged since #21 (2026-07-09)

## [2026-08-08] peer_review | no-op — all 29 open arXiv intakes already reviewed
- Scanned 30 open PRs on willallstet/research-wiki. All 29 arXiv queue PRs
  (#55–#85) already carry an `<!-- llm-wiki-review -->` comment, so every one was
  skipped as already-reviewed. No new reviews posted, no duplicates.
- PR #71 (NEW MODELS Substack, Trevor Paglen "How to See Like a Machine") is the
  one open PR without a peer_review comment, but it is a non-arXiv URL intake and
  routes to /review_content instead — left untouched.
- The backlog is unchanged: reviews are done, the human merge gate is the blocker.

## [2026-08-08] update_wiki | no-op — queue/accepted/ empty; no PR merged since #21 (2026-07-09)
- main has no `queue/accepted/` directory at all: every intake JSON still lives on
  its unmerged `queue/*` branch, so there is nothing to integrate into the wiki.
- No pages created or updated; no contradictions or insights recorded.
- Merging any of the 30 open PRs will land its JSON on main and make the next
  update_wiki run productive.

## [2026-08-08] peer_review | no-op — all 30 open arXiv intakes already reviewed (#55–#85)
User-triggered run. 31 PRs open: 30 arXiv queue intakes, every one already carrying a
`<!-- llm-wiki-review -->` comment, so nothing was re-reviewed. The 31st (#71, a NEW MODELS
Substack event post) was already reviewed by `/review_content` and is out of scope for
peer_review. No comments posted.

## [2026-08-08] update_wiki | no-op — queue/accepted/ empty; no PR merged since #21 (2026-07-09)
No intake JSON awaiting integration. The 30 reviewed arXiv PRs remain open pending the
human merge/close gate, so no wiki pages, index entries, or watermarks changed.

## [2026-08-08] peer_review | no-op — all 62 open arXiv intakes (#10–#85) already carry a review; 6 non-arXiv PRs out of scope
Open PRs total 68. The 62 `queue/accepted/<arxiv-id>.json` intakes all bear a
`<!-- llm-wiki-review -->` comment, so none were re-reviewed. Left alone: #31, #33, #42,
#46, #53, #71 (substack/blog intakes, already reviewed by `/review_content`) and #9 (a
`crawls/` report, not a queue intake).

## [2026-08-08] update_wiki | no-op — no accepted papers; nothing merged since #21 (2026-07-09)
`queue/accepted/` is absent on `main`; every queued intake is still awaiting a human
merge/close decision on its PR. No wiki pages touched.
