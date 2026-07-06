# Comparing Rule-Based, Supervised, and Unsupervised Approaches for Anomaly Detection in System Logs

## Author

**Tamani Williams**  
Master of Science in Computer Science (Artificial Intelligence)  
Troy University

---

## Research Information

**Course:** CS 6625 Specialized Study  
**Instructor:** Dr. Long Ma  
**Term:** Term 5, 2026  
**Status:** In Progress

---

## Abstract

This research investigates the effectiveness of traditional rule-based monitoring compared to supervised and unsupervised machine learning approaches for anomaly detection in distributed system logs. Using the HDFS (Hadoop Distributed File System) dataset, the study evaluates Rule-Based Detection, Logistic Regression, Random Forest, and Isolation Forest models. Performance is measured using accuracy, precision, recall, and F1 score to determine whether machine learning approaches can improve anomaly detection performance over static threshold-based methods.

---

## Overview

This repository contains the code, datasets, experiments, and research artifacts associated with this study.

Each notebook represents one stage of the experimental pipeline, allowing every step of the study to be reproduced independently from raw data preparation through final model evaluation.

---

## Dataset

This study utilizes the **HDFS_v1** dataset, a benchmark dataset widely used in anomaly detection research for distributed systems.

To support reproducibility, an archival mirror of the dataset is maintained at:

https://www.kaggle.com/datasets/tamaniwilliams/hdfs-v1-loghub-dataset-archive

The archive contains:

- HDFS.log
- HDFS.npz
- Event_occurrence_matrix.csv
- Event_traces.csv
- HDFS.log_templates.csv
- anomaly_label.csv

The primary files used throughout this study are:

- Event_occurrence_matrix.csv
- anomaly_label.csv

These files provide the feature matrix and ground truth labels used for evaluating rule-based, supervised, and unsupervised anomaly detection approaches.

---

## Repository Structure

```text
data/
├── raw/
├── processed/

notebooks/

src/

results/

paper/
```

- **data/** contains the original dataset and generated feature sets.
- **notebooks/** contains the complete experimental workflow.
- **src/** contains reusable Python utilities.
- **results/** contains exported evaluation metrics, learned parameters, and model outputs.
- **paper/** contains research planning documents and manuscript materials.

---

## Generated Data

The processed feature sets and train/test split files are not included in this repository because they exceed GitHub's file size limits.

After cloning the repository, generate the required datasets by running the notebooks in the following order:

1. `02_feature_engineering.ipynb`
2. `03_model_preparation.ipynb`

These notebooks recreate:

```text
data/processed/
├── feature_set_1.csv
├── feature_set_2.csv
├── feature_set_3.csv
├── feature_set_4.csv
└── splits/
```

The generated datasets are stored locally and are intentionally excluded from version control.

---

## Project Workflow

Run the notebooks in the following order:

1. `01_data_exploration.ipynb`
2. `02_feature_engineering.ipynb`
3. `03_model_preparation.ipynb`
4. `04_statistical_baseline.ipynb`
5. `05_logistic_regression.ipynb`
6. `06_random_forest.ipynb`
7. `07_isolation_forest.ipynb`
8. `08_results_comparison.ipynb`

---

## Project Status

**Current Phase:** Supervised Model Development

### Completed

- Research topic approved
- Project plan approved
- HDFS_v1 dataset acquisition
- Data exploration
- Feature engineering
- Model preparation
- Statistical rule-based baseline
- Logistic Regression implementation

### In Progress

- Random Forest implementation

### Upcoming

- Isolation Forest implementation
- Cross-model performance comparison
- Final research paper

---

## Results

Model evaluation is performed using the following metrics:

- Accuracy
- Precision
- Recall
- F1 Score

The statistical baseline establishes a traditional rule-based benchmark, while the machine learning models are evaluated using the same engineered feature sets to enable direct performance comparisons.

Final comparative results across all approaches will be presented after completion of the Random Forest and Isolation Forest experiments.

---

## References

1. Wei Xu, Ling Huang, Armando Fox, David Patterson, Michael Jordan. *Detecting Large-Scale System Problems by Mining Console Logs.* Proceedings of the 22nd ACM Symposium on Operating Systems Principles (SOSP), 2009.

2. Jieming Zhu, Shilin He, Pinjia He, Jinyang Liu, Michael R. Lyu. *LogHub: A Large Collection of System Log Datasets for AI-driven Log Analytics.* IEEE International Symposium on Software Reliability Engineering (ISSRE), 2023.

3. Zhihan Jiang, Jinyang Liu, Junjie Huang, Yichen Li, Yintong Huo, Jiazhen Gu, Zhuangbin Chen, Jieming Zhu, Michael R. Lyu. *A Large-scale Evaluation for Log Parsing Techniques: How Far are We?* ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA), 2024.

---

## License

This repository is intended for academic research and educational purposes.

The HDFS dataset is distributed by the LogHub project and remains subject to its original licensing and usage terms.