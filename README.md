# Unsupervised Learning

This repository is dedicated to **Unsupervised Learning**. The goal is to provide educational and practical resources for clustering algorithms and dimensionality reduction techniques (e.g., PCA). The repo currently contains theory documentation and method explanations that are useful for teaching; example notebooks and results will be added and linked here as they become available.

---

##  Current Status
- **Project stage:** Under active development.
- **Documentation:** Theory notes and method explanations for clustering and dimensionality reduction are available in `docs/` and `notebooks/`.
- **Notebooks / Code:** Initial notebooks and examples exist; more practical implementations (KMeans, DBSCAN, PCA) will be added soon.
- **Results:** Visualizations and experiment outputs will be added to `reports/figures` and linked from notebooks.

---

##  Project Structure (planned)
```
Unsupervised-Learning/
├── data/                      # Dataset files (CSV)
├── docs/                      # Theory notes, method explanations
├── notebooks/                 # Jupyter notebooks (clustering, PCA, examples)
│   ├── clustering/
│   └── dimensionality_reduction/
├── src/                       # Reusable source code / modules
├── reports/                   # Reports and figures (results & visualizations)
├── requirements.txt           # Python dependencies
└── README.md                  # This file
```

---

##  Datasets
- Example to load a CSV in a notebook:
```python
import pandas as pd
df = pd.read_csv("data/my_data.csv")  # replace with your file name
df.head()
```

---

## Documentation & Teaching Purpose
- This repo emphasizes **explanations** of algorithms and methods (intended for students/self-learning).
- Each method has a short theory note and an example notebook that demonstrates usage and intuition.
- When experiments are run, results (plots, metrics) will be stored in `reports/figures` and referenced from the corresponding notebook.

---

## Contact
Owner: Mohsen Safari — https://github.com/MohsenSafari83
