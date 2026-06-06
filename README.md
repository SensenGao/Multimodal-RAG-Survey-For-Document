# Scaling Beyond Context: A Survey of Multimodal Retrieval-Augmented Generation for Document Understanding

<p align="center">
  <b>ACL 2026 Main Conference</b>
</p>

<p align="center">
  <a href="https://arxiv.org/abs/2510.15253"><img src="https://img.shields.io/badge/arXiv-2510.15253-b31b1b.svg" alt="arXiv"></a>
  <a href="https://sensengao.github.io/Multimodal-RAG-Survey/"><img src="https://img.shields.io/badge/Project-Page-blue.svg" alt="Project Page"></a>
  <a href="https://github.com/SensenGao/Multimodal-RAG-Survey-For-Document"><img src="https://img.shields.io/github/stars/SensenGao/Multimodal-RAG-Survey-For-Document?style=social" alt="GitHub Stars"></a>
</p>

<p align="center">
  <a href="https://sensengao.github.io/">Sensen Gao</a><sup>1*</sup>,
  <a href="https://sshan-zhao.github.io/">Shanshan Zhao</a><sup>2&dagger;</sup>,
  Xu Jiang<sup>3</sup>,
  <a href="https://github.com/LHDuan">Lunhao Duan</a><sup>4*</sup>,
  <a href="https://scholar.google.com/citations?user=PB7FPEMAAAAJ">Yong Xien Chng</a><sup>3*</sup>,
  <br>
  <a href="https://scholar.google.com/citations?user=GlqRHLcAAAAJ">Qing-Guo Chen</a><sup>2</sup>,
  <a href="https://scholar.google.com/citations?user=tsKl9GUAAAAJ">Weihua Luo</a><sup>2</sup>,
  <a href="https://scholar.google.com/citations?user=e3gpYTYAAAAJ">Kaifu Zhang</a><sup>2</sup>,
  <a href="https://jwbian.net/">Jia-Wang Bian</a><sup>1</sup>,
  <a href="https://mingming-gong.github.io/">Mingming Gong</a><sup>1,5&dagger;</sup>
</p>

<p align="center">
  <sup>1</sup>MBZUAI &nbsp;
  <sup>2</sup>Alibaba International Digital Commerce Group &nbsp;
  <sup>3</sup>Tsinghua University &nbsp;
  <sup>4</sup>Wuhan University &nbsp;
  <sup>5</sup>University of Melbourne
</p>

<p align="center">
  <sub>* Work done during an internship at Alibaba International Digital Commerce Group. &dagger; Corresponding authors.</sub>
</p>

---

<p align="center">
  <img src="assets/home.png" width="54%" alt="Multimodal RAG for Document Understanding">
</p>

This repository maintains a curated list of **methods**, **datasets**, and **benchmarks** for Multimodal Retrieval-Augmented Generation (RAG) in Document Understanding, based on our ACL 2026 survey. We will keep updating this list. Feel free to open an issue or PR if we missed any relevant work!

## Updates

- **2026.04** - Paper accepted at **ACL 2026 Main Conference**!
- **2025.10** - Paper available on [arXiv](https://arxiv.org/abs/2510.15253).

## Table of Contents

- [Overview](#overview)
- [Methods](#methods)
  - [Open-Domain Methods](#open-domain-methods)
  - [Closed-Domain Methods](#closed-domain-methods)
  - [Graph-based Methods](#graph-based-methods)
  - [Agent-based Methods](#agent-based-methods)
- [Datasets & Benchmarks](#datasets--benchmarks)
  - [Document Understanding Datasets](#document-understanding-datasets)
  - [Multimodal RAG Benchmarks](#multimodal-rag-benchmarks)
- [Citation](#citation)

## Overview

<p align="center">
  <img src="assets/overview.png" width="95%">
</p>
<p align="center"><b>A taxonomy of multimodal RAG for document understanding</b>: retrieval <b>domain</b> (open vs. closed), retrieval <b>modality</b> (image vs. image+text), retrieval <b>granularity</b> (page- vs. element-level), and hybrid <b>graph-/agent-based</b> enhancements.</p>

## Methods

### Open-Domain Methods

| Method | Venue | Modality | Granularity | Training | Paper |
|--------|-------|----------|-------------|----------|-------|
| DSE | EMNLP 2024 | Image | Page | Yes | [Link](https://arxiv.org/abs/2406.11251) |
| ColPali | ICLR 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2407.01449) |
| ColQwen2 | ICLR 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2407.01449) |
| VisRAG | ICLR 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2410.10594) |
| M3DocRAG | Preprint | Image | Page | No | [Link](https://arxiv.org/abs/2411.04952) |
| VisDoMRAG | NAACL 2025 | Image+Text | Page | No | [Link](https://arxiv.org/abs/2412.10704) |
| GME | CVPR 2025 | Image+Text | Page | Yes | [Link](https://arxiv.org/abs/2412.16855) |
| ViDoRAG | EMNLP 2025 | Image+Text | Page | No | [Link](https://arxiv.org/abs/2502.18017) |
| HM-RAG | ACM MM 2025 | Image+Text | Page | No | [Link](https://arxiv.org/abs/2504.12330) |
| VDocRAG | CVPR 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2504.09795) |
| VRAG-RL | Preprint | Image | Element | Yes | [Link](https://arxiv.org/abs/2505.22019) |
| CoRe-MMRAG | ACL 2025 | Image+Text | Page | Yes | [Link](https://arxiv.org/abs/2506.02544) |
| Light-ColPali | ACL 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2506.04997) |
| MM-R5 | Preprint | Image | Page | Yes | [Link](https://arxiv.org/abs/2506.12364) |
| SimpleDoc | Preprint | Image+Text | Page | No | [Link](https://arxiv.org/abs/2506.14035) |
| DocVQA-RAP | ICIC 2025 | Image | Element | No | [Link](https://link.springer.com/chapter/10.1007/978-981-96-9921-6_31) |
| RL-QR | Preprint | Image | Page | Yes | [Link](https://arxiv.org/abs/2507.23242) |
| Patho-AgenticRAG | Preprint | Image | Page | Yes | [Link](https://arxiv.org/abs/2508.02258) |
| M2IO-R1 | Preprint | Image+Text | Page | Yes | [Link](https://arxiv.org/abs/2508.06328) |
| mKG-RAG | Preprint | Image+Text | Element | Yes | [Link](https://arxiv.org/abs/2508.05318) |
| DB3Team-RAG | Preprint | Image+Text | Page | Yes | [Link](https://arxiv.org/abs/2509.09681) |
| PREMIR | EMNLP 2025 | Image+Text | Element | No | [Link](https://arxiv.org/abs/2508.17079) |
| CMRAG | Preprint | Image+Text | Page | No | [Link](https://arxiv.org/abs/2509.02123) |
| MoLoRAG | EMNLP 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2509.07666) |
| SERVAL | Preprint | Image | Page | No | [Link](https://arxiv.org/abs/2509.15432) |
| MetaEmbed | Preprint | Image | Page | Yes | [Link](https://arxiv.org/abs/2509.18095) |
| DocPruner | Preprint | Image | Page | Yes | [Link](https://arxiv.org/abs/2509.23883) |
| RECON | Preprint | Image+Text | Element | No | [Link](https://openreview.net/forum?id=nbjsM4zFPG) |
| LAD-RAG | Preprint | Image+Text | Element | No | [Link](https://arxiv.org/abs/2510.07233) |
| HEAVEN | Preprint | Image | Page | No | [Link](https://arxiv.org/abs/2510.22215) |
| MARA | ACM MM 2025 | Image | Element | Yes | [Link](https://arxiv.org/abs/2604.16313) |
| HPC-ColPali | Preprint | Image | Page | Yes | [Link](https://arxiv.org/abs/2506.21601) |
| RegionRAG | Preprint | Image | Element | Yes | [Link](https://arxiv.org/abs/2510.27261) |
| IndustryRAG | EMNLP Industry 2025 | Image | Page | No | [Link](https://aclanthology.org/2025.emnlp-industry.173/) |
| COLMATE | EMNLP Industry 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2511.00903) |
| LILaC | EMNLP 2025 | Image | Element | No | [Link](https://arxiv.org/abs/2602.04263) |
| HKRAG | Preprint | Image | Element | Yes | [Link](https://arxiv.org/abs/2511.20227) |
| SLEUTH | Preprint | Image | Page | No | [Link](https://arxiv.org/abs/2511.22850) |
| Snappy | Preprint | Image | Element | No | [Link](https://arxiv.org/abs/2512.02660) |

### Closed-Domain Methods

| Method | Venue | Modality | Granularity | Training | Paper |
|--------|-------|----------|-------------|----------|-------|
| CREAM | ACM MM 2024 | Image+Text | Page | Yes | [Link](https://arxiv.org/abs/2403.00816) |
| SV-RAG | ICLR 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2411.01106) |
| FRAG | Preprint | Image | Page | No | [Link](https://arxiv.org/abs/2504.17447) |
| MG-RAG | Preprint | Image+Text | Element | No | [Link](https://arxiv.org/abs/2505.01457) |
| VisChunk | Preprint | Image+Text | Page | No | [Link](https://arxiv.org/abs/2506.16035) |
| MMRAG-DocQA | Preprint | Image+Text | Element | No | [Link](https://arxiv.org/abs/2508.00579) |
| ReDocRAG | ICDAR WML 2025 | Image | Page | Yes | [Link](https://arxiv.org/abs/2508.18984) |
| DREAM | ACM MM 2025 | Image | Page | Yes | [Link](https://dl.acm.org/doi/10.1145/3746027.3755357) |
| HEAR | ACM MMW 2025 | Image+Text | Page | No | [Link](https://dl.acm.org/doi/10.1145/3746027.3761999) |

### Graph-based Methods

| Method | Venue | Key Idea | Paper |
|--------|-------|----------|-------|
| HM-RAG | ACM MM 2025 | Hierarchical multi-agent framework with graph databases for structured relation capture | [Link](https://arxiv.org/abs/2504.12330) |
| mKG-RAG | Preprint | Multimodal knowledge graphs aligning entities across vision and text | [Link](https://arxiv.org/abs/2508.05318) |
| DB3Team-RAG | Preprint | Image-indexed knowledge graphs for domain-specific retrieval | [Link](https://arxiv.org/abs/2509.09681) |
| MoLoRAG | EMNLP 2025 | Page graphs encoding logical connections via graph traversal | [Link](https://arxiv.org/abs/2509.07666) |
| RECON | Preprint | Global multimodal document graph linking intra-page and inter-page relations | [Link](https://openreview.net/forum?id=nbjsM4zFPG) |
| LAD-RAG | Preprint | Layout-aware component graphs with dynamic traversal | [Link](https://arxiv.org/abs/2510.07233) |
| LILaC | EMNLP 2025 | Layered component graph with late interaction subgraph retrieval | [Link](https://arxiv.org/abs/2602.04263) |

### Agent-based Methods

| Method | Venue | Key Idea | Paper |
|--------|-------|----------|-------|
| ViDoRAG | EMNLP 2025 | Iterative agent workflow with exploration, summarization, and reflection | [Link](https://arxiv.org/abs/2502.18017) |
| HM-RAG | ACM MM 2025 | Hierarchical multi-agent with query decomposition and consistency voting | [Link](https://arxiv.org/abs/2504.12330) |
| Patho-AgenticRAG | Preprint | Task decomposition and multi-turn search for pathology textbooks | [Link](https://arxiv.org/abs/2508.02258) |
| HEAR | ACM MMW 2025 | Closed-loop multi-agent reasoning with VLM-based document parsing | [Link](https://dl.acm.org/doi/10.1145/3746027.3761999) |
| SLEUTH | Preprint | Coarse-to-fine agent filtering and distilling salient evidence | [Link](https://arxiv.org/abs/2511.22850) |

## Datasets & Benchmarks

### Document Understanding Datasets

| Dataset | #Queries | #Docs/Images | Content | Paper |
|---------|----------|--------------|---------|-------|
| TabFQuAD | 210 | 210 (I) | Table | [Link](https://huggingface.co/datasets/vidore/tabfquad_test_subsampled) |
| PlotQA | 28.9M | 224K (I) | Chart | [Link](https://arxiv.org/abs/1909.00997) |
| DocVQA | 50K | 12,767 (I) | Text, Table, Chart | [Link](https://arxiv.org/abs/2007.00398) |
| VisualMRC | 30,562 | 10,197 (I) | Text, Table, Chart | [Link](https://arxiv.org/abs/2101.11272) |
| TAT-DQA | 16,558 | 2,758 (D) | Text, Table, Chart | [Link](https://arxiv.org/abs/2207.11871) |
| InfoVQA | 30K | 5.4K (I) | Text, Table, Chart | [Link](https://arxiv.org/abs/2104.12756) |
| ChartQA | 23.1K | 17.1K (I) | Chart | [Link](https://arxiv.org/abs/2203.10244) |
| ScienceQA | 21K | 7,803 (I) | Text, Table, Chart | [Link](https://arxiv.org/abs/2209.09513) |
| DUDE | 41,491 | 4,974 (D) | Text, Table, Chart | [Link](https://arxiv.org/abs/2305.08455) |
| SlideVQA | 52K | 14.5K (I) | Slide | [Link](https://arxiv.org/abs/2301.04883) |
| ArXivQA | 100K | 16.6K (D) | Text, Table, Chart | [Link](https://arxiv.org/abs/2403.00231) |
| MMLongBench-Doc | 1,062 | 130 (D) | Text, Table, Chart, Slide | [Link](https://arxiv.org/abs/2407.01523) |
| PaperTab | 393 | 307 (D) | Text, Table | [Link](https://arxiv.org/abs/2406.15187) |
| FetaTab | 1,023 | 878 (D) | Table | [Link](https://arxiv.org/abs/2406.15187) |
| SPIQA | 27K | 25.5K (D) | Table, Chart | [Link](https://arxiv.org/abs/2407.09413) |
| LongDocURL | 2,325 | 396 (D) | Text, Table, Chart | [Link](https://arxiv.org/abs/2412.18424) |

### Multimodal RAG Benchmarks

| Benchmark | #Queries | #Docs/Images | Content | Introduced By | Paper |
|-----------|----------|--------------|---------|---------------|-------|
| ViDoRe | 3.8K | 8.3K (D) | Text, Table, Chart | ColPali | [Link](https://arxiv.org/abs/2407.01449) |
| VisR-Bench | 471 | 226 (D) | Text, Table, Chart, Slide | VisR-Bench | [Link](https://arxiv.org/abs/2508.07493) |
| M3DocVQA | 2,441 | 3,368 (D) | Text, Table, Chart | M3DocRAG | [Link](https://arxiv.org/abs/2411.04952) |
| VisDoMBench | 2,271 | 1,277 (D) | Text, Table, Chart, Slide | VisDoMRAG | [Link](https://arxiv.org/abs/2412.10704) |
| ViDoSeek | 1,142 | 300 (D) | Text, Table, Chart | ViDoRAG | [Link](https://arxiv.org/abs/2502.18017) |
| OpenDocVQA | 206K | 43K (I) | Text, Table, Chart | VDocRAG | [Link](https://arxiv.org/abs/2504.09795) |
| UniDoc-Bench | 1.6K | 70K (I) | Text, Table, Chart | UniDoc | [Link](https://arxiv.org/abs/2510.03663) |
| BBox-DocVQA | 32K | 4.4K (D) | Text, Table, Chart | BBox-DocVQA | [Link](https://arxiv.org/abs/2511.15090) |

## Citation

If you find this survey useful, please cite our paper:

```bibtex
@article{gao2025scaling,
      title={Scaling Beyond Context: A Survey of Multimodal Retrieval-Augmented Generation for Document Understanding},
      author={Sensen Gao and Shanshan Zhao and Xu Jiang and Lunhao Duan and Yong Xien Chng and Qing-Guo Chen and Weihua Luo and Kaifu Zhang and Jia-Wang Bian and Mingming Gong},
      year={2025},
      eprint={2510.15253},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2510.15253},
}
```

## Contact

For questions or suggestions, feel free to open an issue or contact [Sensen Gao](mailto:sensen.gao@mbzuai.ac.ae).
