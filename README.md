# DL for Cybersecurity — Lab Series

Deep learning models applied to real cybersecurity problems. Three independent labs, each tackling a different security domain with a progressively more complex architecture.

---

## Labs

### 1. FFNN — Network Intrusion Detection
**Folder:** `ffnn_network_intrusion/`

Binary and multi-class intrusion detection on network traffic data (CICIDS2017 dataset). Covers the full ML pipeline from data preprocessing to hyperparameter tuning.

**Covered:** Shallow FFNN · Deep FFNN · ReLU vs Linear activation · Feature bias analysis (Destination Port) · Class imbalance with weighted loss · Batch size & optimizer comparison · Weight decay regularization

**Stack:** Python · PyTorch · Scikit-learn · Pandas · Matplotlib

---

### 2. FFNN / RNN / GNN — Malware Detection via API Call Sequences
**Folder:** `ffnn_rnn_gnn_malware/`

Malware detection from sequences of Windows API calls. Compares multiple architectures across the same problem to understand the trade-offs between model complexity and performance.

**Covered:** Frequency-based baseline (Logistic Regression) · Sequential ID vs Learnable Embedding FFNN · One-directional RNN · Bidirectional RNN · Bi-LSTM · GCN · GraphSAGE · GAT

**Stack:** Python · PyTorch · PyTorch Geometric · Scikit-learn · Pandas · Matplotlib

---

### 3. NLP / BERT — SSH Log Analysis & MITRE Tactic Tagging
**Folder:** `nlp_bert_ssh_analysis/`

Named Entity Recognition (NER) on SSH honeypot logs. Fine-tunes pre-trained language models to classify each bash command with its corresponding MITRE ATT&CK tactic, then applies the model to 170k real-world attack sessions.

**Covered:** Dataset characterization · BERT vs UnixCoder tokenization · Pre-trained vs naked BERT · BERT vs UnixCoder fine-tuning · Frozen fine-tuning strategies · Inference on unlabeled data · Attack fingerprint analysis over time

**Stack:** Python · PyTorch · Hugging Face Transformers · BERT · UnixCoder · Scikit-learn · Matplotlib

---

## Datasets

| Lab | Dataset | Source |
|-----|---------|--------|
| 1 | CICIDS2017 | [University of New Brunswick](https://www.unb.ca/cic/datasets/ids-2017.html) |
| 2 | Malware API Call Sequences | [Kaggle](https://www.kaggle.com/datasets/ang3loliveira/malware-analysis-datasets-api-call-sequences) |
| 3 | SSH Honeypot Sessions (CyberLab) | Politecnico di Torino — not publicly redistributable |

> Datasets are not included in this repository. See the links above for labs 1 and 2.

---

## Structure

```
dl-cybersecurity-labs/
├── ffnn_network_intrusion/
│   ├── ffnn.ipynb
│   └── ffnn.pdf
├── ffnn_rnn_gnn_malware/
│   ├── rnn_gnn.ipynb
│   └── rnn_gnn.pdf
├── nlp_bert_ssh_analysis/
│   ├── nlp.ipynb
│   └── nlp.pdf
└── README.md
```

---

## Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
