# Stats 201 Mini Project — Micro-Expression Analysis

This repo is a lightweight scaffold to run basic system checks and load a small **sample** micro-expression dataset.

## Environments

### A) Google Colab (cloud, easiest)
1. Open a new notebook in Colab.
2. Upload this project zip or clone from your storage.
3. Run:
   ```python
   %cd /content/<project-folder>
   !pip -q install -r requirements.txt
   ```
4. Open `code/system_and_data_demo.ipynb` and run all.

### B) AWS EC2 or AWS SageMaker Studio
- **EC2 (Ubuntu 22.04):**
  ```bash
  sudo apt update && sudo apt -y install python3-pip python3-venv
  python3 -m venv .venv && source .venv/bin/activate
  python -m pip install --upgrade pip
  pip install -r requirements.txt
  jupyter lab
  ```
- **SageMaker Studio:** Create a Python 3 (PyTorch) kernel and run:
  ```bash
  pip install -r requirements.txt
  ```

### C) Local (conda)
```bash
conda create -n stats201 python=3.10 -y
conda activate stats201
pip install -r requirements.txt
jupyter lab
```

## Project layout
```
.
├── README.md
├── requirements.txt
├── data
│   ├── sample_microexpressions.csv
│   └── README.md
└── code
    └── system_and_data_demo.ipynb
```

## Notes
- The dataset here is a **small synthetic sample** shaped after public micro-expression benchmarks (CASME II, SAMM, SMIC, CASME3) to avoid license friction while you wait for approvals. Replace it with real files later.
- GPU is optional; the notebook detects CUDA if available.
