<h1 align="center">ASWANI SAHOO</h1>

<p align="center">
  <a href="https://github.com/AswaniSahoo">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&repeat=true&width=435&height=25&lines=ML+%26+AI+Systems+Engineer;Agentic+Tool+Execution;Verifiable+Runtimes;Scientific+ML" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/AswaniSahoo"><img src="https://img.shields.io/badge/33_Upstream_Merged_PRs-181717?style=for-the-badge&logo=github&logoColor=white" alt="33 Upstream Merged PRs"/></a>
  <a href="https://github.com/pytorch"><img src="https://img.shields.io/badge/PyTorch_Org_Member-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch Org Member"/></a>
  <a href="https://github.com/AswaniSahoo/climate-risk-agent/pkgs/container/climate-ipcc-rag-mcp"><img src="https://img.shields.io/badge/Live_MCP_Container-0052CC?style=for-the-badge&logo=docker&logoColor=white" alt="Live MCP Container"/></a>
  <a href="https://x.com/AswaniSahoo2"><img src="https://img.shields.io/badge/@AswaniSahoo2-000000?style=for-the-badge&logo=x&logoColor=white" alt="Twitter"/></a>
  <a href="https://linkedin.com/in/aswani-sahoo/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
</p>

---

### About

Building production ML systems and verifiable agentic runtimes: deterministic verification gates, Model Context Protocol (MCP) infrastructure, atmospheric forecasting, and scientific ML.  
Self-taught ML systems engineer from a non-CS background (Ceramic Engineering): built verifiable runtimes, shipped 33 merged PRs upstream, and earned PyTorch organization membership.

**B.Tech Ceramic Engineering @ NIT Rourkela ('27)** | **CGPA: 8.02** | Odisha, India

---

### Open Source: 33 Merged Upstream PRs

<table>
<tr>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/pytorch/pytorch/pulls?q=is%3Apr+is%3Aclosed+author%3AAswaniSahoo">
<img src="https://img.shields.io/badge/PyTorch-5_merged-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch"/>
</a>
</h4>

- **Docathon 2026:** Honorable Mention ("First-timer", Rank 7 of 33, 17 pts)
- Migrated 5 core documentation modules to MyST Markdown (`nn.functional`, `autograd`, `extending.func`, `mkldnn`, `gradcheck`)
- Resolved cross-referencing errors and sphinx build warnings in PyTorch core docs pipeline
- Key PRs: [#182925](https://github.com/pytorch/pytorch/pull/182925), [#182626](https://github.com/pytorch/pytorch/pull/182626)

</td>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/pytorch/executorch/pulls?q=is%3Apr+author%3AAswaniSahoo+is%3Aclosed">
<img src="https://img.shields.io/badge/ExecuTorch-4_merged-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="ExecuTorch"/>
</a>
</h4>

- Fixed broken `{include}` paths rendering 3 empty backend documentation pages
- Documented manual CMake build and `ctest` workflow for C++ test execution
- Added top-of-page Memory Inspector API usage example with `print_data_tabular()`
- Key PRs: [#19585](https://github.com/pytorch/executorch/pull/19585), [#19386](https://github.com/pytorch/executorch/pull/19386), [#19387](https://github.com/pytorch/executorch/pull/19387)

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/openclimatefix/graph_weather/pulls?q=is%3Apr+author%3AAswaniSahoo+is%3Aclosed">
<img src="https://img.shields.io/badge/Open_Climate_Fix-19_merged-2E8B57?style=flat-square&logo=github&logoColor=white" alt="Open Climate Fix"/>
</a>
</h4>

- <strong>Root-Caused Decoder Persistence Collapse:</strong> Traced model failure to discarded encoder features and zero-seeded decoder observation nodes. Shipped zero-parameter skip-connection fix (PR #237, #239), lifting held-out forecasting skill from 4% to <strong>20% over persistence</strong>.
- <strong>Movable Adaptive Meshing Architecture:</strong> Shipped <code>DynamicGraphBuilder</code>, <code>RegionalForecaster</code>, and <code>BoundaryNudgingLayer</code> for arbitrary runtime sub-grid weather forecasting.
- <strong>Published Negative Result (Issue #238):</strong> Ran controlled 3-seed held-out ablation proving a 19k-parameter per-node MLP outperformed 2.27M-parameter GNN meshes; detailed scaling and coupling tradeoffs.
- <strong>Co-credited Contributor:</strong> Formal credit in <code>graph_weather</code> v1.0.132 release (Zenodo DOI).
- Key PRs: [#166](https://github.com/openclimatefix/graph_weather/pull/166), [#181](https://github.com/openclimatefix/graph_weather/pull/181), [#221](https://github.com/openclimatefix/graph_weather/pull/221), [#237](https://github.com/openclimatefix/graph_weather/pull/237), [#239](https://github.com/openclimatefix/graph_weather/pull/239)

</td>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/krkn-chaos/krkn-ai/pulls?q=is%3Apr+author%3AAswaniSahoo">
<img src="https://img.shields.io/badge/CNCF_%2F_krkn--chaos-3_merged-FF6600?style=flat-square&logo=kubernetes&logoColor=white" alt="CNCF / krkn-chaos"/>
</a>
</h4>

- Fixed fitness function range-query window covering full test duration in `krkn-ai`
- Synchronized `uv.lock` with pinned development dependencies across CI runs
- Resolved missing scenario frontmatter `weight` definitions on docs website
- Key PRs: [#378](https://github.com/krkn-chaos/krkn-ai/pull/378), [#374](https://github.com/krkn-chaos/krkn-ai/pull/374), [#476](https://github.com/krkn-chaos/website/pull/476)

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/malariagen/malariagen-data-python/pulls?q=is%3Apr+is%3Aclosed+author%3AAswaniSahoo">
<img src="https://img.shields.io/badge/MalariaGEN_%2F_Sanger-2_merged-1E90FF?style=flat-square&logo=github&logoColor=white" alt="MalariaGEN Sanger Institute"/>
</a>
</h4>

- Added lower-triangle pairwise population fixation index ($F_{ST}$) heatmap visualization for vector genomics
- Resolved CNV data verification indentation defect preventing silent execution errors
- Key PRs: [#969](https://github.com/malariagen/malariagen-data-python/pull/969), [#895](https://github.com/malariagen/malariagen-data-python/pull/895)

</td>
<td width="50%" valign="top">

<h4>
<img src="https://img.shields.io/badge/Active_Focus-Upstream-6E40C9?style=flat-square&logo=github&logoColor=white" alt="Active Focus"/>
</h4>

- **[Open Climate Fix / graph_weather](https://github.com/openclimatefix/graph_weather/issues/3):** Adaptive meshing, dual-graph prototype for regional NWP, dynamic encoder graphs
- **[KubeEdge / Ianvs](https://github.com/kubeedge/ianvs/pulls?q=is%3Apr+author%3AAswaniSahoo):** Edge AI benchmarking CI modernization and dependency fixes
- **[krkn-chaos / krkn-ai](https://github.com/krkn-chaos/krkn-ai/pulls?q=is%3Apr+author%3AAswaniSahoo):** Automated chaos scenario discovery and node label filtering

</td>
</tr>
</table>

---

### Flagship Systems & Production Artifacts

<table>
<tr>
<td width="100%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/Incident-evidence-compiler">Incident Evidence Compiler (IEC)</a></h4>
<p><em>Automated Root Cause Analysis (RCA) on telemetry via deterministic verification graphs and LLM hypothesis generation.</em></p>

<p>
  <img src="https://img.shields.io/badge/Tests-304_passed-success?style=flat-square" alt="304 Tests" />
  <img src="https://img.shields.io/badge/Architecture-Hexagonal_Core-blue?style=flat-square" alt="Hexagonal Core" />
  <img src="https://img.shields.io/badge/Queue-PostgreSQL_SKIP_LOCKED-blueviolet?style=flat-square" alt="PostgreSQL" />
</p>

- <strong>Core Invariant:</strong> LLM proposes hypotheses; only deterministic code decides.
- <strong>Verification Gate:</strong> Hexagonal core with stdlib-only domain behind ports. Hypotheses bounded to observed signals; emits cryptographic verdicts: <code>SUPPORTED</code>, <code>REFUTED</code>, <code>UNKNOWN</code>.
- <strong>Concurrency &amp; Infrastructure:</strong> Async PostgreSQL worker queue using <code>FOR UPDATE SKIP LOCKED</code> for lock-free parallel triage; dependency-free Prometheus <code>/metrics</code>.
- <strong>Sealed RCAEval Benchmark:</strong>
  - Dev Split (RE2-OB, 88 cases): Top-1: <strong>0.932</strong> | Top-3: <strong>0.989</strong> | MRR: <strong>0.959</strong>
  - Held-out Split (RE2-TT, 90 unseen cases): Top-1: <strong>0.767</strong> | Top-3: <strong>0.878</strong> | MRR: <strong>0.833</strong>
  - <strong>0.0% invalid citations</strong>; safely abstained on <strong>52 of 90</strong> held-out cases rather than emit ungrounded causes.
- <strong>Discipline:</strong> 304 automated tests; zero leakages; strict typing; Apache-2.0.

<pre><code>git clone https://github.com/AswaniSahoo/Incident-evidence-compiler.git
cd Incident-evidence-compiler && pytest  # 304 passing tests</code></pre>

</td>
</tr>
</table>

<table>
<tr>
<td width="100%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/climate-risk-agent">Climate-Risk Agent & MCP Infrastructure</a></h4>
<p><em>Evaluated 4-node LangGraph risk intelligence system with split-boundary Model Context Protocol (MCP) servers.</em></p>

<p>
  <img src="https://img.shields.io/badge/Tests-238_passed-success?style=flat-square" alt="238 Tests" />
  <img src="https://img.shields.io/badge/Registry-io.github.AswaniSahoo%2Fclimate--ipcc--rag-blue?style=flat-square" alt="MCP Registry" />
  <img src="https://img.shields.io/badge/GHCR-Live_Container-blueviolet?style=flat-square" alt="GHCR" />
</p>

- <strong>Production Container:</strong> Published on GHCR and indexed on official MCP Registry as <code>io.github.AswaniSahoo/climate-ipcc-rag</code>.
- <strong>Split MCP Security Boundary:</strong>
  - <code>weather-mcp</code>: Live weather forecast routines + 60+ yr ERA5 Generalized Extreme Value (GEV) hazard statistics (bootstrap 90% CIs).
  - <code>ipcc-rag-mcp</code>: Hybrid BM25 + dense Reciprocal Rank Fusion (RRF) over IPCC AR6 WG I & II reports with page citations.
- <strong>Protocol Security:</strong> <code>ToolAnnotations</code> (<code>read_only_hint=True</code>, <code>open_world_hint=True</code>); measured client-sandbox credential isolation in MCP Inspector.
- <strong>Frozen Held-Out Evaluation (105 Questions):</strong>
  - Retrieval: Recall@3: <strong>87.0%</strong> | Recall@5: <strong>91.0%</strong> | Recall@10: <strong>96.2%</strong>
  - Grounding: <strong>94.0% citation validity</strong>; <strong>0.0% false answers</strong> on refusal confusion matrix; ~$0.001 per grounded report.
- <strong>Discipline:</strong> 238 unit and integration tests.

<pre><code>docker pull ghcr.io/aswanisahoo/climate-ipcc-rag-mcp:0.1.0</code></pre>

</td>
</tr>
</table>

---

### Engineered Systems & Applied Machine Learning

<table>
<tr>
<td width="50%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/fairness-credit-risk">Fairness & Statistical Honesty</a></h4>
<p>
  <img src="https://img.shields.io/badge/Tests-235_passed-success?style=flat-square" alt="235 Tests" />
  <img src="https://img.shields.io/badge/Focus-Fair_ML_%26_ECOA-blue?style=flat-square" alt="Fair ML" />
</p>

- Evaluated 5 algorithmic intervention tracks (T0 through T4) on credit risk scoring across shared seeded splits with compliance guardrails.
- **Published Negative Result:** Proved no algorithmic intervention improved disparate impact without violating ECOA / Regulation B non-discrimination mandates.
- **Foundation Model Benchmark:** 1.6B parameter TabFM failed to outperform tuned GBDT at ~1,000x compute cost.
- **Discipline:** 235 automated tests covering statistical parity, equalized odds, and audit logs.

</td>
<td width="50%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/weather-transformer-scratch">Weather Transformer from Scratch</a></h4>
<p>
  <img src="https://img.shields.io/badge/Tests-74_passed-success?style=flat-square" alt="74 Tests" />
  <img src="https://img.shields.io/badge/Framework-Pure_PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="Pure PyTorch" />
</p>

- Physics-aware Vision Transformer built completely from scratch in pure PyTorch without using <code>torch.nn.MultiheadAttention</code>.
- Custom spatial-temporal patch embeddings, spherical coordinate encodings, and physics-constrained continuity loss on ERA5 data.
- **Empirical Gain:** <strong>+27% RMSE improvement</strong> over operational persistence baseline on 6-hour atmospheric forecasting.
- **Discipline:** 74 unit tests validating attention matrix shapes, gradient flow, and energy conservation.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/llama-task-agent">LLaMA Task Agent</a></h4>
<p>
  <img src="https://img.shields.io/badge/Model-LLaMA--3.1--8B-blue?style=flat-square&logo=meta&logoColor=white" alt="LLaMA" />
  <img src="https://img.shields.io/badge/Tuning-LoRA_%2F_PEFT-EE4C2C?style=flat-square" alt="LoRA" />
</p>

- Parameter-efficient fine-tuning (LoRA / PEFT) of LLaMA-3.1-8B for deterministic agentic tool execution.
- Maps unstructured natural language task instructions into type-safe, schema-validated JSON function calls with zero syntax defects.
- Enforces strict argument validation across complex multi-turn execution graphs.

</td>
<td width="50%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/complaint-intelligence-system">Complaint Intelligence System</a></h4>
<p>
  <img src="https://img.shields.io/badge/Data-200K+_Complaints-informational?style=flat-square" alt="200K Complaints" />
  <img src="https://img.shields.io/badge/Interface-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit" />
</p>

- High-throughput RAG pipeline indexing over 200,000+ CFPB consumer financial complaints using hybrid FAISS vector search and LLMs.
- **Latency Benchmark:** Quantified latency versus semantic coherence: MiniLM (p95: <strong>41ms</strong>) vs BGE (p95: <strong>1356ms</strong>).
- Deployed with interactive Streamlit exploration UI and automated cluster analysis.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/biodiversity-publication-analyzer">Bio Publication Analyzer</a></h4>
<p>
  <img src="https://img.shields.io/badge/Tests-81_passed-success?style=flat-square" alt="81 Tests" />
  <img src="https://img.shields.io/badge/Accuracy-99.5%25_F1-brightgreen?style=flat-square" alt="99.5% F1" />
</p>

- SciBERT + TF-IDF ensemble text classification pipeline for genomics and biodiversity literature.
- Achieved <strong>99.5% F1 score</strong> on Europe PMC open-access biomedical corpus.
- **Discipline:** 81 unit tests ensuring deterministic feature tokenization and inference stability.

</td>
<td width="50%" valign="top">

<h4><a href="https://github.com/AswaniSahoo/malariagen-nlp-interface-poc">MalariaGEN NLP Interface</a></h4>
<p>
  <img src="https://img.shields.io/badge/Validation-10%2F10_Queries-success?style=flat-square" alt="10/10 Queries" />
  <img src="https://img.shields.io/badge/Domain-Genomics_API-1E90FF?style=flat-square" alt="Genomics API" />
</p>

- Natural language query translation layer for vector genomics data (`malariagen_data` API).
- Validated 10 of 10 test queries with automated parameter binding across 7 public genomic exploration API methods.
- Bridges domain scientific queries with complex underlying dataframes and visualization routines.

</td>
</tr>
</table>

---

### Tech Stack & Tooling

<p align="center">
  <img src="https://skillicons.dev/icons?i=pytorch,python,docker,linux,git,fastapi,postgres,github,vscode&theme=dark&perline=9" alt="Core Skills" />
</p>

<p align="center">
  <strong>Agentic Tooling & Verifiable Systems</strong><br/>
  <img src="https://img.shields.io/badge/Model_Context_Protocol-MCP-0052CC?style=flat-square&logo=anthropic&logoColor=white" alt="MCP" />
  <img src="https://img.shields.io/badge/LangGraph-State_Machines-FF6B6B?style=flat-square&logo=langchain&logoColor=white" alt="LangGraph" />
  <img src="https://img.shields.io/badge/Pydantic_v2-Schema_Validation-E92063?style=flat-square&logo=pydantic&logoColor=white" alt="Pydantic" />
  <img src="https://img.shields.io/badge/PostgreSQL-SKIP_LOCKED_Queues-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Prometheus-Metrics-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus" />
  <img src="https://img.shields.io/badge/Docker-Multi--Arch_GHCR-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
</p>

<p align="center">
  <strong>Scientific Machine Learning & Scaled Retrieval</strong><br/>
  <img src="https://img.shields.io/badge/PyTorch-Deep_Learning-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
  <img src="https://img.shields.io/badge/HuggingFace-Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="HuggingFace" />
  <img src="https://img.shields.io/badge/LoRA%2FPEFT-Fine--Tuning-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="LoRA/PEFT" />
  <img src="https://img.shields.io/badge/FAISS-Vector_Search-0467DF?style=flat-square&logo=meta&logoColor=white" alt="FAISS" />
  <img src="https://img.shields.io/badge/xarray-Atmospheric_Tensors-E34F26?style=flat-square&logo=python&logoColor=white" alt="xarray" />
  <img src="https://img.shields.io/badge/zarr-Chunked_Storage-2C2255?style=flat-square&logo=python&logoColor=white" alt="zarr" />
  <img src="https://img.shields.io/badge/SciBERT-Biomedical_NLP-4285F4?style=flat-square&logo=google-scholar&logoColor=white" alt="SciBERT" />
  <img src="https://img.shields.io/badge/SciPy-GEV_Hazard_Modeling-8CAAE6?style=flat-square&logo=scipy&logoColor=white" alt="SciPy" />
</p>

---

### GitHub Streak & Activity

<p align="center">
  <img width="60%" src="https://github-readme-streak-stats.herokuapp.com?user=AswaniSahoo&theme=tokyonight&hide_border=true" alt="Aswani Sahoo GitHub Streak" />
</p>

---

### Background & Credentials

- **Education:** B.Tech Ceramic Engineering, National Institute of Technology, Rourkela (2023 - 2027) | **CGPA: 8.02**
- **Certifications:**
  - Oracle Cloud Infrastructure 2025 Generative AI Professional
  - Oracle Cloud Infrastructure 2025 Data Science Professional
  - Oracle Cloud Infrastructure 2025 AI Foundations Associate

---

<p align="center">
  <a href="mailto:aswanisahoo227@gmail.com"><img src="https://img.shields.io/badge/aswanisahoo227@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>
