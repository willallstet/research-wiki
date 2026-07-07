---
source: arxiv/2607.04461
commit: n/a
files: [https://arxiv.org/abs/2607.04461]
updated: 2026-07-07
kind: paper
interesting: 4/5
---

# Flash-BoN: Instant Drafts for Inference-Time Scaling in Diffusion Models

**arXiv:** [2607.04461](https://arxiv.org/abs/2607.04461) · **Authors:** Ruchit Rawal,
Reza Shirkavand, Sayak Paul, Yuxin Wen, Heng Huang, Yizheng Chen, Tom Goldstein,
Gowthami Somepalli (UMD; Hugging Face) · **Published:** 2026-07-05 · cs.CV

A reading tracked for its relevance to [[ai-and-machine-vision]] — specifically the
mechanics of **text-to-image generation**, one of Will's documented interests.

## What it argues

Inference-time scaling for text-to-image (T2I) diffusion generates many candidate
images and picks the best via a verifier. The paper makes two claims:

1. **Wall-clock, not NFEs.** The field's standard compute metric — number of
   function evaluations — undercounts verifier overhead. Measured by real
   wall-clock time, simple **Best-of-N** already matches or beats sophisticated
   guided-search methods (BFS/DFS/ZOS), whose frequent intermediate verification
   eats the time budget.
2. **Generation cost is a spendable axis.** *Flash-BoN* makes cheap "draft"
   candidates (early-stopping + layer-skipping + Taylor-expansion activation
   proxies, calibrated once per model by dual-annealing optimization), scores them
   with a multi-stage pointwise→pairwise (Elo) verifier, and refines only the
   winner at full quality.

Across 3 benchmarks × 3 model scales it leads every cell, with gains widening at
larger scale (+8% AUC); the draft idea also transfers to RL post-training
(Flash-Flow-GRPO, ~10× fewer gradient steps to match). A notable honest finding:
using ImageReward as both verifier and evaluator inflates gains (+270%) via reward
over-optimization — the model "locks onto a narrow aesthetic," which resonates with
Will's critical take on how image models encode a predetermined viewpoint.

## Why it's here

- **Concept fit:** [[ai-and-machine-vision]] — text-to-image generation, plus the
  verifier/reward-model aesthetic-bias thread.
- **Assessment:** peer-reviewed in-repo (PR #1, recommendation *accept*; overall 4/5).
  Strength: a correct measurement reframing backed by broad experiments and honest
  negative results. Weakness: no error bars on headline numbers; the core mechanism
  repurposes existing accelerators rather than introducing a new one.

Provenance: reviewed from the full 36-page PDF. Source: intake PR #1 (merged).
