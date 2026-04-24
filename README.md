# Reproducing and Extending “The Geometry of Truth”

This repository contains the extended abstract and research findings for a reproduction and extension of Marks & Tegmark’s *"The Geometry of Truth"* (2023). This work was prepared for the **EEML 2026 Reproduction Track**.

## 📄 Research Abstract
We reproduce “The Geometry of Truth” (Marks & Tegmark, 2023), confirming
that Mass-Mean (MM) probes are more causally implicated in representing factual
truth than Logistic Regression (LR) probes in LLaMA-2-13B. However, we reveal
severe generalization vulnerabilities: probes overfit to structural heuristics unless
datasets are perfectly balanced. Extending this work, we evaluate LLaMA-3.1-
8B-Instruct, finding improved native decoupling of numerical and factual truth.
We also demonstrate cross-lingual transfer, evaluating an English-trained probe
on French (97.3%), Spanish (92.0%), and Serbian (76.7%) text. Finally, we test
the probe against the Apollo Deception dataset (Goldowsky-Dill et al., 2025). It
completely fails to distinguish honest from deceptive prompts, suggesting linear
truth probes detect objective semantic correlations rather than strategic intent.

## 🚀 Key Technical Extensions
*   **Model Scaling:** Evaluated truth-direction emergence in **LLaMA-3.1-8B-Instruct**, identifying Layer 10 as a critical information bottleneck.
*   **Strategic Deception:** Tested linear truth probes against the **Apollo Deception dataset**, demonstrating that factual probes detect objective semantic correlations rather than internal strategic intent.
*   **Cross-Lingual Transfer:** Verified that internal representations of truth are largely language-agnostic, with strong zero-shot transfer from English to French, Spanish, and Serbian.

## 💻 Infrastructure & Engineering
*   **Hardware:** Experiments were conducted on **NVIDIA A100** GPUs provisioned via **Vast.ai**.
*   **CUDA Optimization:** To handle high-dimensional hidden state extraction (LLaMA-2-13B), the covariance matrix inversion and PCA pipeline were migrated from CPU (MKL) to **CUDA**, resolving memory bottlenecks and accelerating the processing pipeline.

## 📊 Repository Status
- [x] Extended Abstract (PDF)
- [ ] Codebase Refactoring (In Progress)
- [ ] Analysis Notebooks (In Progress)

*Note: The core codebase is currently being refactored for public release to ensure code quality and reproducibility standards.*

## References
Marks, S., & Tegmark, M. (2023). The Geometry of Truth: Emergent Linear Structure in Large Language Model Representations of Truth/False Datasets.
