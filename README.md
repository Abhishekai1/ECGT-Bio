# ECGT-Bio: Explainable Counterfactual Graph Transformer for Biomedical Discovery

> **Status**: Research Prototype — Designed for publication in top-tier AI/ML venues (e.g., NeurIPS, ICLR, AAAI, ICML).

## 📌 Overview
**ECGT-Bio** is a **novel AI framework** that fuses **graph neural networks**, **causal inference**, and **domain-specific knowledge** to enable *explainable, counterfactual reasoning* over **biomedical knowledge graphs**.

Unlike conventional link prediction models, ECGT-Bio is built to:
- **Predict** new biomedical relationships (drug–disease, gene–phenotype, protein–interaction).
- **Explain** *why* the prediction is made, using subgraph evidence.
- **Simulate interventions** — *What if this gene was silenced? What if a drug targeted a different pathway?*
- **Quantify uncertainty**, enabling trust in high-stakes biomedical applications.

---

## 🚀 Research Contributions

1. **Graph Transformer Backbone**  
   A heterogeneous Graph Transformer with attention-based multi-relation message passing.

2. **Counterfactual Reasoning Module**  
   `do()`-style interventions for causal simulation of biomedical scenarios.

3. **Uncertainty-Aware Predictions**  
   Outputs calibrated confidence intervals using heteroscedastic modeling.

4. **Neuro-Symbolic Rule Integration**  
   Embeds biomedical knowledge constraints directly into the loss function.

5. **Invariant Risk Minimization (IRM)**  
   Ensures robustness across dataset shifts and experimental biases.

---

## 🧪 Applications
- **Drug Repurposing**: Identify unexpected drug–disease links.
- **Genetic Target Discovery**: Explore therapeutic targets through simulated knockouts.
- **Clinical Trial Prioritization**: Rank candidates with explainable evidence and uncertainty scores.

---

## 📊 Experimental Highlights
Evaluated on both **synthetic causal biomedical KGs** and **Hetionet** (real-world KG with 47k+ entities, 2.2M+ edges):

| Model           | AUC ↑  | AP ↑   | ECE ↓  | CCS ↑ |
|-----------------|--------|--------|--------|-------|
| R-GCN           | 0.902  | 0.884  | 0.081  | 0.41  |
| CompGCN         | 0.908  | 0.889  | 0.079  | 0.43  |
| GT (Baseline)   | 0.918  | 0.903  | 0.072  | 0.48  |
| + Rules         | 0.936  | 0.921  | 0.061  | 0.59  |
| + IRM           | 0.927  | 0.913  | 0.066  | 0.54  |
| **Full Model**  | **0.949** | **0.937** | **0.052** | **0.63** |
---

## 📈 Visualizations
- **ROC & PR curves** for predictive performance.
- **Calibration plots** for uncertainty quality.
- **UMAP embeddings** to visualize learned biomedical space.
- **Subgraph explanations** for predictions.
- **Counterfactual heatmaps** for intervention impact.

---

## 📜 Citation
bibtex
@misc{ecgtbio2025,
  title={ECGT-Bio: Explainable Counterfactual Graph Transformer for Biomedical Discovery},
  author={Abhishek Yadav},
  year={2025},
  howpublished={GitHub},
}
---

