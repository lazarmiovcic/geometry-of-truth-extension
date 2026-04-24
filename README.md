# Reproducing and Extending “The Geometry of Truth”

This repository contains the extended abstract and research findings for a reproduction and extension of Marks & Tegmark’s *"The Geometry of Truth"* (2023). This work was prepared for the **EEML 2026 Reproduction Track**.

## 📄 Research Abstract
[Copy and paste the abstract text from your PDF here]

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
