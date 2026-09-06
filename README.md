<div align="center">

# Aswani Sahoo
**ML & AI Systems Engineer** | Agentic Tool Execution · Verifiable Runtimes · Scientific ML  
**33 merged upstream PRs** across PyTorch (5), ExecuTorch (4), graph_weather (19), krkn-chaos (3), MalariaGEN (2)  
**PyTorch Docathon 2026 Honorable Mention** (Rank 7 of 33, 17 pts) | **Live MCP Container:** `ghcr.io/aswanisahoo/climate-ipcc-rag-mcp:0.1.0`

[GitHub](https://github.com/AswaniSahoo) · [LinkedIn](https://linkedin.com/in/aswani-sahoo/) · [Email](mailto:aswanisahoo227@gmail.com) · NIT Rourkela (2023 - 2027, CGPA: 8.02)

</div>

---

### Core Systems & Production Artifacts

#### 1. [Incident Evidence Compiler (IEC)](https://github.com/AswaniSahoo/Incident-evidence-compiler)
> **Automated Root Cause Analysis (RCA) on incident telemetry using deterministic graphs and verifier-gated LLMs.**  
> *Core invariant: An LLM is allowed to propose hypotheses; only deterministic code is allowed to decide.*

- **Verification Gate Architecture:** Hexagonal core with stdlib-only domain behind ports. Hypotheses from Gemini are strictly bounded to an allow-list of observed telemetry signals. A deterministic verifier evaluates content-addressed evidence ledgers and emits only cryptographically backed verdicts: `SUPPORTED`, `REFUTED`, or `UNKNOWN`.
- **Infrastructure & Concurrency:** Async PostgreSQL worker queue utilizing `FOR UPDATE SKIP LOCKED` for lock-free parallel incident triage; FastAPI control plane with constant-time bearer token auth and tenant scoping; dependency-free Prometheus `/metrics` endpoint tracking stage latency and verdict distributions.
- **Sealed Benchmark Evaluation (RCAEval Benchmark):**
  - **Dev Split (RE2-OB, 88 cases):** Baseline Top-1: **0.932** | Top-3: **0.989** | MRR: **0.959**.
  - **Sealed Held-Out Split (RE2-TT, 90 unseen cases, commit `0a7854e`):** Baseline Top-1: **0.767** | Top-3: **0.878** | MRR: **0.833**.
  - **Citation Integrity:** **0.0% invalid evidence citations** across both model generations (`gemini-2.5-flash` and `gemini-3.7-flash`). Safely abstained on **52 of 90** held-out cases rather than emit an unverified failure cause.
- **Test Discipline:** 304 automated tests running with zero network, database, or mock leakage; full `mypy --strict` compliance; Apache-2.0.

```bash
# Clone and verify test suite (304 passing tests)
git clone https://github.com/AswaniSahoo/Incident-evidence-compiler.git
cd Incident-evidence-compiler && pytest
```

---

#### 2. [Climate-Risk Agent & MCP Infrastructure](https://github.com/AswaniSahoo/climate-risk-agent)
> **Evaluated 4-node LangGraph risk intelligence system with split-boundary Model Context Protocol (MCP) servers.**

- **Production Multi-Arch Container:** Published on GitHub Container Registry and indexed on the official Model Context Protocol Registry as `io.github.AswaniSahoo/climate-ipcc-rag`.
- **Split MCP Security Boundary:** Implemented two distinct MCP servers over `stdio` transport (`mcp==2.0.0`):
  - `weather-mcp`: Exposes live weather forecast routines and 60+ year ERA5 Generalized Extreme Value (GEV) hazard statistics (stationary and non-stationary models with likelihood-ratio trend tests and 90% bootstrap confidence intervals).
  - `ipcc-rag-mcp`: Hybrid BM25 and dense Reciprocal Rank Fusion (RRF) retrieval over IPCC AR6 Working Group I & II reports with page-level citation validation.
- **Protocol Engineering & Sandbox Security:**
  - Full adherence to `ToolAnnotations`: Explicit `read_only_hint=True` and `open_world_hint=True` with hardcoded coordinate bounding.
  - Measured client-sandbox credential isolation in MCP Inspector: Identified client environment variable stripping and engineered fallback via non-destructive `load_dotenv(override=False)`.
- **Empirical Rigor (105-Question SHA-256 Frozen Held-Out Test):**
  - **Retrieval Performance:** Recall@3: **87.0%** | Recall@5: **91.0%** | Recall@10: **96.2%**.
  - **Grounding & Guardrails:** **94.0% citation validity**; **0.0% false answers** on refusal confusion matrix.
  - **Efficiency:** Telemetry recorded at ~$0.001 per grounded report; 238 unit and integration tests.

```bash
# Pull and inspect the production MCP container from GHCR
docker pull ghcr.io/aswanisahoo/climate-ipcc-rag-mcp:0.1.0
```

---

### Empirical Rigor & Statistical Honesty

- **[fairness-credit-risk](https://github.com/AswaniSahoo/fairness-credit-risk):** Evaluated 5 intervention tracks (T0 through T4) across shared seeded splits with 235 unit and integration tests. Published an honest negative finding: no algorithmic intervention improved disparate impact without violating Equal Credit Opportunity Act (ECOA) / Regulation B compliance, and a 1.6B parameter Tabular Foundation Model (TabFM) did not distinguishably outperform a tuned GBDT while incurring approximately 1,000x compute cost.
- **[weather-transformer-scratch](https://github.com/AswaniSahoo/weather-transformer-scratch):** Physics-aware Vision Transformer built completely from scratch in PyTorch without using `torch.nn.MultiheadAttention`. Implements custom spatial-temporal patch embedding, spherical coordinate encodings, and physics-constrained continuity loss on ERA5 data. Tested via 74 unit tests; achieved a 27% RMSE improvement over the persistence baseline.

---

### Upstream Open Source Track Record (33 Merged PRs)

| Organization / Repository | Merged | Technical Scope & Production Impact | Verification |
|:---|:---:|:---|:---|
| **[PyTorch Core](https://github.com/pytorch/pytorch)** (`pytorch/pytorch`) | **5** | Migrated core documentation to MyST Markdown (`nn.functional`, `autograd`, `extending.func`, `mkldnn`, `gradcheck`). Ranked **#7 of 33** in PyTorch Docathon 2026 (Honorable Mention, designated "First-timer", 17 pts). | [#182925](https://github.com/pytorch/pytorch/pull/182925), [#182626](https://github.com/pytorch/pytorch/pull/182626) |
| **[PyTorch ExecuTorch](https://github.com/pytorch/executorch)** (`pytorch/executorch`) | **4** | Embedded edge runtime docs and build verification: fixed broken include paths, added Memory Inspector API examples with `print_data_tabular()`, documented manual CMake and `ctest` workflow. | [#19585](https://github.com/pytorch/executorch/pull/19585), [#19386](https://github.com/pytorch/executorch/pull/19386), [#19387](https://github.com/pytorch/executorch/pull/19387) |
| **[Open Climate Fix](https://github.com/openclimatefix/graph_weather)** (`openclimatefix/graph_weather`) | **19** | Implemented `ThermalizerLayer` diffusion modeling, NNJA-AI V1 dataset loader, variable-resolution H3 mesh generators, dynamic bipartite graph builders, and `RegionalForecaster`. Published controlled 3-seed ablation in issue #238. Co-credited in v1.0.132 release. | [#166](https://github.com/openclimatefix/graph_weather/pull/166), [#171](https://github.com/openclimatefix/graph_weather/pull/171), [#181](https://github.com/openclimatefix/graph_weather/pull/181), [#221](https://github.com/openclimatefix/graph_weather/pull/221) |
| **[CNCF / krkn-chaos](https://github.com/krkn-chaos/krkn-ai)** (`krkn-chaos/krkn-ai`, `website`) | **3** | Fixed fitness function range-query window covering full test duration, synchronized `uv.lock` with pinned dev dependencies, and resolved scenario frontmatter weight definitions. | [#378](https://github.com/krkn-chaos/krkn-ai/pull/378), [#374](https://github.com/krkn-chaos/krkn-ai/pull/374), [#476](https://github.com/krkn-chaos/website/pull/476) |
| **[MalariaGEN](https://github.com/malariagen/malariagen-data-python)** (`malariagen/malariagen-data-python`) | **2** | Added lower-triangle pairwise population fixation index ($F_{ST}$) heatmap visualization; resolved CNV data verification indentation defect preventing silent execution errors. | [#969](https://github.com/malariagen/malariagen-data-python/pull/969), [#895](https://github.com/malariagen/malariagen-data-python/pull/895) |

---

### Systems Depth & Technical Skills

| Domain | Core Competencies & Proven Tooling |
|:---|:---|
| **Agentic Tooling & Verifiable Runtimes** | Model Context Protocol (MCP, `ToolAnnotations`, MCP Registry), LangGraph state machines, Deterministic Verification Gates, Cryptographic Evidence Ledgers, Pydantic v2 schemas |
| **Deep Learning & ML Systems** | PyTorch from-scratch tensor primitives, Parameter-Efficient Fine-Tuning (LoRA, QLoRA via PEFT), Vision Transformers, Graph Neural Networks (message passing, bipartite graphs), Hugging Face Transformers |
| **Distributed Runtimes & Infrastructure** | Async FastAPI, PostgreSQL (`FOR UPDATE SKIP LOCKED` concurrent worker queues), Multi-Arch Docker (GHCR), Dependency-Free Prometheus `/metrics`, GitHub Actions CI/CD, Linux, CMake |
| **Scientific Computing & Scaled Retrieval** | ERA5 atmospheric reanalysis, GEV extreme value statistical modeling (scipy), xarray, zarr, FAISS vector search, BM25, Reciprocal Rank Fusion (RRF), Cross-Encoder reranking |

---

### Background & Credentials

- **Education:** B.Tech Ceramic Engineering, National Institute of Technology, Rourkela (2023 - 2027) | **CGPA: 8.02**
- **Certifications:**
  - Oracle Cloud Infrastructure 2025 Generative AI Professional
  - Oracle Cloud Infrastructure 2025 Data Science Professional
  - Oracle Cloud Infrastructure 2025 AI Foundations Associate
