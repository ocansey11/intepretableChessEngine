
# Interpretable and Explainable Chess Engine
### Author
**Kevin Ocansey**  
Email: [kevinocansey11@gmail.com]  
Kaggle: [kevinocansey]([https://www.kaggle.com/kevinocansey](https://www.kaggle.com/code/kevinocansey/interpretable-and-explainable-chess-engine))

---


## Overview

This repository contains the full code, models, and supporting materials for my final dissertation: **"Interpretable and Explainable Chess Engine: Deep Learning, Concept Discovery, and XAI for Neural Chess Policies"**. The project explores how modern deep neural networks can be made more transparent and interpretable in the context of chess, combining state-of-the-art supervised learning with advanced explainability techniques.

- **Core notebook:** `interpretable-and-explainable-chess-engine.ipynb`
- **Pre-trained models:** ResNet-50, DenseNet-121, VGG-16 (12-plane and 19-plane encodings)
- **Data:** Preprocessed Lichess positions with Stockfish annotations
- **XAI methods:** SHAP, TCAV, Integrated Gradients, Saliency Maps
- **Visuals:** Architecture diagrams, feature importance heatmaps, and more (see `images/`)
- **Literature:** Extensive collection of research papers on chess AI and explainability (see `papers/`)

---

## Project Structure

- `submission Ocansey Kevin/`
  - `interpretable-and-explainable-chess-engine.ipynb` – Main notebook (full pipeline, experiments, and analysis)
  - `positions_with_sf.parquet` – Preprocessed dataset (subset for QUICK_START)
  - `*_best.pt` – Pre-trained model checkpoints (ResNet, DenseNet, VGG)
  - `README.md` – Data access and reproducibility instructions
- `images/` – Diagrams, architecture visualizations, and result plots
- `papers/` – Research papers, literature reviews, and supporting documents

---

## Key Features

- **Multi-architecture training:** Compare ResNet-50, DenseNet-121, and VGG-16 on chess move prediction
- **Flexible input encoding:** 12-plane (basic) and 19-plane (with rule context) board representations
- **Comprehensive interpretability:** SHAP, TCAV, and gradient-based methods for concept discovery and model explanation
- **Reproducibility:** QUICK_START mode for lightweight testing, full dataset available via Kaggle
- **Rich visualizations:** Feature importance, concept heatmaps, architecture diagrams, and more

---

## Getting Started

### QUICK_START (Recommended for Reviewers)

1. Place `positions_with_sf.parquet` and all `*_best.pt` model files in the same directory as the notebook.
2. Open `interpretable-and-explainable-chess-engine.ipynb`.
3. Set `QUICK_START = True` in the notebook.
4. Run all cells. The notebook will use the provided data and pre-trained models for fast, reproducible results.

### Full Reproducibility

- Download the full Lichess dataset (≈30GB) from [Kaggle](https://www.kaggle.com/datasets/kevinocansey/lichess-data-february-standard-rated-2025).
- Follow the instructions in the notebook to preprocess, train, and analyze from scratch.

---

## Folders & Contents

- **images/**: Visual summaries, architecture diagrams, feature importance, and result plots.
- **papers/**: Key research papers, literature reviews, and supporting material on chess AI and explainability.
- **submission Ocansey Kevin/**: All code, models, and data needed for review and reproduction.

---

## Research Questions

1. How accurately can neural chess engines predict moves compared to benchmark engines when trained on Lichess data?
2. Which interpretability techniques best reveal human-understandable chess concepts from internal representations?
3. How consistently do different interpretability methods identify the same concepts for given positions?
4. What can be learned about how deep neural networks represent and develop chess concepts during training?

---

## Citation

If you use this code, models, or analysis in your own research, please cite this dissertation or contact me for collaboration opportunities.

---


## Acknowledgements

- Emili Balanguer, classmates, Edward, Adwoa, Yuli, Gerald Joachim and the chess AI research community
- Lichess for providing the open chess dataset

---

For detailed instructions on running the notebook and accessing data, see `submission Ocansey Kevin/README.md`.
