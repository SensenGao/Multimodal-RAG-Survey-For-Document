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
  Shanshan Zhao<sup>2&dagger;</sup>,
  Xu Jiang<sup>3</sup>,
  Lunhao Duan<sup>4*</sup>,
  Yong Xien Chng<sup>3*</sup>,
  <br>
  Qing-Guo Chen<sup>2</sup>,
  Weihua Luo<sup>2</sup>,
  Kaifu Zhang<sup>2</sup>,
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
  <img src="assets/home.png" width="90%" alt="Multimodal RAG for Document Understanding">
</p>

## Overview

Document understanding is critical for applications from financial analysis to scientific discovery. Current approaches face key limitations: OCR-based pipelines lose structural detail, while native Multimodal LLMs struggle with context modeling. **Multimodal RAG** enables holistic retrieval and reasoning across all modalities (text, tables, charts, and layout), unlocking comprehensive document intelligence.

This survey presents the **first comprehensive study** that explicitly bridges multimodal RAG and document understanding, covering:

- **Taxonomy** based on domain (open/closed), retrieval modality, granularity, and hybrid enhancements
- **Graph-based** and **agent-based** frameworks for structured reasoning
- **Datasets, benchmarks**, and comparative evaluations
- **Applications** in finance, science, social analysis, and industry deployment
- **Open challenges** and future research directions

## Taxonomy

<p align="center">
  <img src="assets/domain.png" width="85%" alt="Open vs Closed Domain">
</p>
<p align="center"><b>Open-domain vs. closed-domain multimodal RAG.</b></p>

<p align="center">
  <img src="assets/mode.png" width="85%" alt="Retrieval Modality">
</p>
<p align="center"><b>Retrieval modality: image-based vs. image+text-based.</b></p>

<p align="center">
  <img src="assets/ret_level.png" width="85%" alt="Retrieval Granularity">
</p>
<p align="center"><b>Retrieval granularity: page-level vs. element-level.</b></p>

<p align="center">
  <img src="assets/Graph_Agent.png" width="85%" alt="Graph and Agent based RAG">
</p>
<p align="center"><b>Hybrid enhancements: graph-based and agent-based multimodal RAG.</b></p>

## Key Dimensions

| Dimension | Categories | Description |
|-----------|-----------|-------------|
| **Domain** | Open / Closed | Open-domain retrieves from large corpora; closed-domain focuses on single documents |
| **Retrieval Modality** | Image / Image+Text | Image-only via VLM encoders vs. hybrid with OCR/captions |
| **Retrieval Granularity** | Page / Element | Whole-page retrieval vs. fine-grained tables, charts, layout blocks |
| **Graph Enhancement** | Knowledge Graphs / Page Graphs | Structured reasoning via multimodal knowledge graphs |
| **Agent Enhancement** | Single / Multi-Agent | Autonomous query decomposition, retrieval orchestration, and verification |

## Updates

- **2026.05** - Paper accepted at **ACL 2026 Main Conference**!
- **2025.10** - Paper available on [arXiv](https://arxiv.org/abs/2510.15253).

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

## Acknowledgements

This work was supported by MBZUAI, Alibaba International Digital Commerce Group, Tsinghua University, Wuhan University, and the University of Melbourne.

## Contact

For questions or suggestions, feel free to open an issue or contact [Sensen Gao](mailto:sensen.gao@mbzuai.ac.ae).
