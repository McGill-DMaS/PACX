# PAC-X: Fuzzy Explainable AI for Multi-Class Malware Detection

**License:** Apache-2.0  
**Status:** Research code release  
**Authors:** Saqib et al.  

---

If you find this project useful, please cite:



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

## 📂 Repository Structure (top-level)
PACX/
├── data/                    # Dataset files
├── prospect/               # Prospect analysis modules
├── PACX_explainability_prospect_aspect_fixindices.py
├── explainability_context.py
├── explainability_prospect_aspect.py
├── fuzzySetGenrator.py     # Fuzzy set generation
├── fuzzySetGenrator_group.py
├── pac-x.py               # Main PAC-X implementation
├── testing.py             # Testing scripts
├── testing_ttd.py         # Time-to-detection testing
├── training.py            # Training scripts
├── training_binary.py     # Binary classification training
├── training_without_CANNET.py
├── utility.py             # Utility functions
└── LICENSE


---

## 🏁 Quick Start

> *(Add installation, environment, and run commands here later)*

---

## 🏷️ License

This project is released under the **Apache-2.0 License**.  
See the `LICENSE` file for details.

---



If you find this project useful, please cite:
> M. Saqib, B. C. M. Fung, and P. Charland.  
> **PAC-X: fuzzy explainable AI for multi-class malware detection**.  
> *IEEE Transactions on Fuzzy Systems (TFS)*, in-press (2025).  
> doi: 10.1109/TFUZZ.2025.3621833. IEEE Press.

---

M. Saqib, B. C. M. Fung, and P. Charland. PAC-X: fuzzy explainable AI for multi-class malware detection. IEEE Transactions on Fuzzy Systems (TFS), in press. IEEE Press.
