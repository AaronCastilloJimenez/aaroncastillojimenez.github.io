---
title: "Automated 3D Segmentation of the Root Meristem"
excerpt: "A high-throughput pipeline utilizing Convolutional Neural Networks (PlantSeg & Cellpose) for characterizing cell geometry and cycle dynamics."
collection: portfolio
header:
  teaser: "https://raw.githubusercontent.com/MouseLand/cellpose/main/cellpose/logo.png"
---

### 🔬 Project Overview
This project addresses the challenge of analyzing complex 3D cellular structures in the *Arabidopsis thaliana* root apical meristem. Currently under development, the pipeline automates the processing of multi-channel confocal stacks to extract precise geometric and temporal data.



---

### 🛠️ Technical Workflow

#### 1. Multi-Channel Processing
The pipeline handles raw `.nd2` (Nikon) files, synchronizing three key biological reporters:
* **Cell Wall (e.g., PI/Renaissance):** Defines the structural scaffold for geometric analysis.
* **Dual Cell-Cycle Reporters:** Visualizes nuclear dynamics at different phases (G1/S/G2/M), allowing for the mapping of proliferation zones.

#### 2. AI-Driven Segmentation
We leverage state-of-the-art **Convolutional Neural Networks (CNNs)** to overcome the limitations of traditional thresholding:
* **PlantSeg:** Provides robust 3D segmentation of cell boundaries from cell wall markers.
* **Cellpose:** Delivers high-fidelity nuclear segmentation, even in dense meristematic regions.

#### 3. Curation & Refinement
* **Napari Integration:** A custom Python-based GUI for real-time proofreading and manual correction.
* **Post-Processing:** Scripts to calculate cell volumes, surface areas, and spatial distribution of cell-cycle states.

---

### 🚀 Key Outcomes
* **Automation:** Drastic reduction in manual annotation time for large datasets.
* **Precision:** High-resolution mapping of cell identity and proliferation patterns.
* **Scale:** Enables the quantitative comparison of wild-type vs. mutant phenotypes at a single-cell level.

---

### 💻 Stack & Tools
| Category | Tools |
| :--- | :--- |
| **Languages** | Python, MATLAB |
| **DL Frameworks** | PyTorch (PlantSeg), Cellpose |
| **Visualization** | Napari, Fiji/ImageJ |
| **Bioinformatics** | ND2SDK, NumPy, SciPy |

[View Project Documentation on GitHub](https://github.com/AaronCastilloJimenez/meta-GRN-Root-Epidermis)
