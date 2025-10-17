# PAC-X: Fuzzy Explainable AI for Multi-Class Malware Detection

## 🧠 What is PAC-X?

Researchers often approach malware detection as a **binary classification** problem.  
However, evidence shows that:

- a malware sample can belong to **multiple families** at the same time  
- malware frequently contains **benign-looking features** to evade detection  
- adversarial perturbations can **fool both classifiers and explanations**

This makes malware detection a **fuzzy multi-class** and **explainability-critical** problem.

**PAC-X solves this** by introducing a novel XAI framework that:

- integrates **CAN-Net** (Conditional Attention Neural Network) for *multi-fuzzy-class explainability*
- uses **Contextual Fuzzy Clustering (CFC)** to extract context-aware fuzzy insights
- remains **robust under adversarial manipulations** that try to distort explanations

Extensive experiments across multiple malware datasets show that PAC-X:

- offers **deeper and more faithful explanations** than state-of-the-art XAI baselines
- is **resilient** against adversarial attempts to mislead the model or its explanations
- advances explainability in real-world evasive malware detection

---

### File Descriptions

- **data/**: Contains dataset files and data processing utilities
- **prospect/**: Modules for prospect analysis and aspect evaluation
- **PACX_explainability_prospect_aspect_fixindices.py**: Explainability module with fixed indices for prospect aspects
- **explainability_context.py**: Implements contextual explainability using fuzzy clustering
- **explainability_prospect_aspect.py**: Prospect theory-based aspect explainability
- **fuzzySetGenrator.py**: Generates fuzzy sets for individual malware features
- **fuzzySetGenrator_group.py**: Group-based fuzzy set generation for feature clusters
- **pac-x.py**: Main implementation of the PAC-X framework
- **testing.py**: Comprehensive testing and evaluation suite
- **testing_ttd.py**: Time-to-detection analysis module
- **training.py**: Main training pipeline with CAN-Net integration
- **training_binary.py**: Binary classification training variant
- **training_without_CANNET.py**: Training without CAN-Net for ablation studies
- **utility.py**: Common utility functions and helper methods
- **LICENSE**: Apache 2.0 license file

---
If you use this work in your research, please cite:

M. Saqib, B. C. M. Fung, and P. Charland. PAC-X: fuzzy explainable AI for multi-class malware detection. IEEE Transactions on Fuzzy Systems (TFS), doi: 10.1109/TFUZZ.2025.3621833, in press. IEEE Press.
