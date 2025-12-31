# DarkPatterns-LLM Benchmark Dataset

This repository hosts the **DarkPatterns-LLM Benchmark Dataset**, a curated dataset for
detecting **manipulative and harmful behaviors in Large Language Model (LLM) outputs**.

The dataset accompanies the paper:

> **DarkPatterns-LLM: A Multi-Layer Benchmark for Detecting Manipulative and Harmful AI Behavior**  
> Sadia Asif, Israel Antonio Rosales Laguan, Haris Khan, Shumaila Asif, Muneeb Asif  
> arXiv preprint, 2025

🔗 **Paper (arXiv)**: https://arxiv.org/abs/2512.22470  
🌐 **Project Website**: https://sadia-sigma-lab.github.io/darkpatterns-llm/

---

## 📌 Overview

Large Language Models increasingly influence high-stakes decisions in domains such as
healthcare, finance, education, and governance. While existing safety benchmarks rely on
coarse binary labels, they fail to capture **subtle, psychologically grounded manipulation
strategies**.

**DarkPatterns-LLM** addresses this gap by providing a **multi-dimensional benchmark**
designed to evaluate manipulative behaviors that undermine user autonomy, trust, and
well-being.

---

## 📂 Dataset Description

The benchmark consists of **401 expert-annotated instruction–response pairs**.
Each instance contains:

- `instruction` — the user prompt or scenario  
- `rejected` — a manipulative or harmful LLM response  
- `accepted` — a safe, non-manipulative alternative response  
- `discussion` — expert rationale explaining the harm and correction  
- `category` — primary harm category label  

---

## 🧠 Harm Taxonomy

Each example is assigned to **one of seven harm categories**:

1. Legal / Power Harm  
2. Psychological Harm  
3. Emotional Harm  
4. Physical Harm  
5. Autonomy Harm  
6. Economic Harm  
7. Societal Harm  

The taxonomy is grounded in psychology, ethics, human–computer interaction, and AI safety
literature on dark patterns and manipulation.

---

## 🧪 Annotation Methodology

- Annotated by **domain experts** in AI safety, psychology, and ethics  
- Includes **paired harmful and safe responses** for contrastive evaluation  
- Inter-annotator agreement: **Fleiss’ κ = 0.68**  
- Cross-cultural review to mitigate cultural bias  
- Automated validation for format consistency and duplication removal  

---

## 🔬 Intended Use

This benchmark is intended for:

- Safety evaluation and benchmarking of LLMs  
- Manipulation and dark pattern detection research  
- Explainable AI safety diagnostics  
- Evaluation of autonomy-preserving AI systems  
- Policy, governance, and regulatory-aligned studies (e.g., EU AI Act)

⚠️ The dataset is **not intended** for training models to generate manipulative content.

---

## 🧩 Evaluation Framework

The dataset supports the four-layer evaluation framework introduced in the paper:

1. **Multi-Granular Detection (MGD)**  
2. **Multi-Scale Intent Analysis (MSIAN)**  
3. **Threat Harmonization Protocol (THP)**  
4. **Deep Contextual Risk Alignment (DCRA)**  

Associated evaluation metrics:
- Manipulation Resistance Index (MRI)  
- Contextual Robustness Score (CRS)  
- Stakeholder Impact Assessment Score (SIAS)  
- Temporal Harm Dynamics Score (THDS)  

---

## 📜 License

This dataset is released under the **Creative Commons Attribution (CC BY 4.0)** license.

You are free to use, modify, and redistribute the dataset **with appropriate attribution**.

---

## 📖 Citation

If you use this dataset, or found our framework helpful, please cite:

```bibtex

@article{darkpatternsllm2025,
  title={DarkPatterns-LLM: A Multi-Layer Benchmark for Detecting Manipulative and Harmful AI Behavior},
  author={Asif, Sadia and Rosales Laguan, Israel Antonio and Khan, Haris and Asif, Shumaila and Asif, Muneeb},
  journal={arXiv preprint arXiv:2512.22470},
  year={2025}
}
