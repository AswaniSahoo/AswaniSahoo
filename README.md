<h1 align="center">ASWANI SAHOO</h1>

<p align="center">
  <a href="https://github.com/AswaniSahoo">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&repeat=true&width=435&height=25&lines=ML+Engineer;Open+Source+Contributor" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/AswaniSahoo"><img src="https://img.shields.io/badge/33_Upstream_Merged_PRs-181717?style=for-the-badge&logo=github&logoColor=white" alt="Merged PRs"/></a>
  <a href="https://github.com/pytorch"><img src="https://img.shields.io/badge/PyTorch_Org_Member-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/></a>
  <a href="https://x.com/AswaniSahoo2"><img src="https://img.shields.io/badge/@AswaniSahoo2-000000?style=for-the-badge&logo=x&logoColor=white" alt="Twitter"/></a>
  <a href="https://linkedin.com/in/aswani-sahoo/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
</p>

---

### About

I build ML systems for science and production: LLM agents with measured evaluation, weather forecasting models, genomics NLP.

Not from a CS background. Taught myself ML, shipped code upstream, earned PyTorch org recognition. Most of what I know came from having patches reviewed by maintainers who did not have to be kind about it.

B.Tech @ NIT Rourkela '27 | CGPA 8.02 | Odisha, India

---

### Open Source: 33 Merged PRs across 5 organizations

<table>
<tr>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/openclimatefix/graph_weather/pulls?q=is%3Apr+author%3AAswaniSahoo+is%3Aclosed">
<img src="https://img.shields.io/badge/Open_Climate_Fix-19_merged-2E8B57?style=flat-square&logo=github&logoColor=white" />
</a>
</h4>

- Built the **adaptive-mesh regional forecasting** stack end to end: `DynamicGraphBuilder`, `RegionalForecaster`, `BoundaryNudgingLayer`, variable-resolution H3 mesh, stretched-grid dataset and region-weighted loss
- Root-caused a silent failure where the decoder discarded the encoder's per-observation features, capping the model at the no-change baseline. Skip-connection fix, **zero new parameters**, held-out skill 4% → 20% over persistence
- Earlier: `ThermalizerLayer` diffusion denoising, NNJA-AI V1 dataset loader
- Listed as contributor in graph_weather **v1.0.132** (Zenodo DOI)

</td>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/pytorch/pytorch/pulls?q=is%3Apr+is%3Aclosed+author%3AAswaniSahoo">
<img src="https://img.shields.io/badge/PyTorch-5_merged-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
</a>
<a href="https://github.com/pytorch/executorch/pulls?q=is%3Apr+author%3AAswaniSahoo+is%3Aclosed">
<img src="https://img.shields.io/badge/ExecuTorch-4_merged-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
</a>
</h4>

- Docathon 2026: **Honorable Mention** (first-timer category)
- Migrated 5 core doc files (`nn.functional`, `autograd`, `extending.func`, `mkldnn`, `gradcheck`) from RST to MyST
- Fixed broken `{include}` paths rendering 3 empty backend pages
- Documented the CMake build + ctest workflow for C++ tests
- Added an Inspector API usage example with `print_data_tabular()`

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/krkn-chaos/krkn-ai/pulls?q=is%3Apr+author%3AAswaniSahoo">
<img src="https://img.shields.io/badge/krkn--chaos_(CNCF)-3_merged-FF6600?style=flat-square&logo=kubernetes&logoColor=white" />
</a>
</h4>

- Fitness-windows bug fix in the chaos-scenario scoring path
- Dependency sync across the krkn-ai toolchain
- Fixed missing `weight` field in network-chaos-ng scenario frontmatters

</td>
<td width="50%" valign="top">

<h4>
<a href="https://github.com/malariagen/malariagen-data-python/pulls?q=is%3Apr+is%3Aclosed+author%3AAswaniSahoo">
<img src="https://img.shields.io/badge/MalariaGEN-2_merged-1E90FF?style=flat-square&logo=github&logoColor=white" />
</a>
</h4>

- Added lower-triangle annotation for Fst heatmaps in the malaria vector genomics library
- Fixed a CNV data-check indentation bug causing silent failures

</td>
</tr>
</table>

<h4>Currently Active</h4>

- [graph_weather #3](https://github.com/openclimatefix/graph_weather/issues/3) / [#238](https://github.com/openclimatefix/graph_weather/issues/238) — adaptive meshing for regional NWP. Currently running a controlled ablation on whether the mesh message-passing earns its parameters against a graph-free baseline; publishing the numbers either way.
- [krkn-chaos/krkn-ai #389](https://github.com/krkn-chaos/krkn-ai/pull/389) — Elasticsearch config for composite chaos scenarios
- [malariagen-data-python #1310](https://github.com/malariagen/malariagen-data-python/pull/1310) — haplotype network mixin

---

### Projects

| Project | What it does | Highlights |
|:--------|:------------|:-----------|
| [Climate-Risk Analyst Agent](https://github.com/AswaniSahoo/climate-risk-agent) — **[live](https://climate-risk-agent-714882950125.us-central1.run.app/)** | LangGraph agent returning typed, cited climate-risk reports — or refusing when the evidence is thin | 105-question SHA-frozen held-out set: recall@3 87%, citation validity 94%, **zero false answers**. 238 tests, ~$0.001/report, deployed on Cloud Run |
| [Incident Evidence Compiler](https://github.com/AswaniSahoo/Incident-evidence-compiler) | Root-cause investigation service where the model proposes and deterministic code decides | **RCAEval RE2-OB**: top-1 0.932, MRR 0.959. Content-addressed evidence ledger, Postgres `SKIP LOCKED` worker queue, 304 hermetic tests, mypy strict |
| [Weather Transformer](https://github.com/AswaniSahoo/weather-transformer-scratch) | Physics-aware Transformer for 6-hour weather forecasting on ERA5 | Written from scratch in PyTorch — no `nn.MultiheadAttention`. 74 tests, beats persistence by **27% RMSE** on a 1,316-sample held-out set |
| [Fairness-Aware Credit Risk](https://github.com/AswaniSahoo/fairness-credit-risk) | Four bias-mitigation interventions measured against a tuned baseline under identical conditions, on two credit datasets | **No intervention helped** — and the reasons differ per dataset. Bootstrap intervals on every metric, **212 tests**, SHAP adverse-action reason codes, model card. Includes a published self-audit of three defects in my own earlier version, including a proxy leak where dropping `gender` did not remove sex from the model. Every published number regenerated from an artifact, enforced by a test |
| [Complaint Intelligence](https://github.com/AswaniSahoo/complaint-intelligence-system) — **[live](https://complaint-intelligence-system.streamlit.app/)** | RAG and retrieval benchmark over CFPB consumer complaints | **200K CFPB complaints** processed end to end. MiniLM vs BGE, vector vs BM25 vs hybrid vs rerank, KMeans vs BERTopic — every component chosen on measured results, not defaults |
| [LLaMA Task Agent](https://github.com/AswaniSahoo/llama-task-agent) | LoRA fine-tuned LLaMA-3.1-8B for agentic tool execution | Generates valid function calls with type-safe args from natural language |
| [Bio Publication Analyzer](https://github.com/AswaniSahoo/biodiversity-publication-analyzer) | SciBERT + TF-IDF classifier for genomics articles | 81 tests, Europe PMC pipeline end to end |

---

### Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=pytorch,python,postgres,docker,linux,git,fastapi,gcp,github,vscode&theme=dark&perline=10" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/HuggingFace_Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/LoRA/PEFT-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white" />
  <img src="https://img.shields.io/badge/xarray-E34F26?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/zarr-2C2255?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/mypy_strict-2A6DB2?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white" />
</p>

---

### GitHub Stats

<p align="center">
  <img width="60%" src="https://github-readme-streak-stats.herokuapp.com?user=AswaniSahoo&theme=tokyonight&hide_border=true" />
</p>

---

<p align="center">
  <a href="mailto:aswanisahoo227@gmail.com"><img src="https://img.shields.io/badge/aswanisahoo227@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>
