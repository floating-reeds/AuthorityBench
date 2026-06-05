# AuthorityBench

**Authority, Truth, and Citation Bias: A Large-Scale Multi-Domain Benchmark for Studying Epistemic Susceptibility in Large Language Models**

AuthorityBench is a large-scale, multi-domain benchmark designed to study how citation-based authority signals shape epistemic behavior in Large Language Models (LLMs). The benchmark uses a fully balanced 2×2 factorial design crossing claim veracity (true vs. false) with citation veracity (real vs. fabricated) across four domains: general knowledge, science, law, and medicine.

## Key Features

- **220,564 Prompts**: The largest citation-authority benchmark, evaluating both citation-induced hallucination and the novel condition of citation-induced denial of correct facts.
- **Multi-Domain**: Covers general knowledge (FEVER), science (SciQ), law (CaseHOLD), and medicine (MedMCQA).
- **Controlled Variation**: Incorporates 40 prompt templates, four venue prestige tiers, and a country-coded author name dataset to control for presentation, prestige, and demographic variables.

## Main Findings

- Adding any citation—fabricated or real—increases hallucination above the no-citation baseline.
- The effect is most extreme when fabricated citations are paired with true claims, raising hallucination rates by 3 to 22 percentage points, reaching up to 77% in the general knowledge domain. 
- Legal claims are comparatively robust, while venue prestige and author demographics show negligible impact.
- Vulnerability to citation-induced hallucination does not track model size or general capability.

## Getting Started

### Prerequisites

Install the required dependencies using:

```bash
pip install -r requirements.txt
```

### Repository Contents

- `inference_pipeline.ipynb`: The notebook for running model inference across the benchmark.
- `evaluator_sop.ipynb`: Standard Operating Procedure (SOP) notebook for the evaluation pipeline.

### Dataset

The dataset can be found at [Dataset Link](https://bitspilaniac-my.sharepoint.com/:f:/g/personal/f20231279_pilani_bits-pilani_ac_in/IgB80e0TSlwLTZ_F8ebxyZdTAXBKVv4e2MuZ3RqHUEHSAn8?e=IGD24D) (password: AuthorityBench)

## Citation

If you use this benchmark in your work, please cite:

```bibtex
@article{authoritybench2026,
  title={Authority, Truth, and Citation Bias: A Large-Scale Multi-Domain Benchmark for Studying Epistemic Susceptibility in Large Language Models},
  author={Aryan Khurana, Aravind Ramana RN, Dhruv Kumar},
  year={2026}
}
```
