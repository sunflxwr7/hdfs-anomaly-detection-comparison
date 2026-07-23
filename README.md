# A Comparative Study of Rule Based, Supervised, and Unsupervised Anomaly Detection for HDFS System Logs

## Author

**Tamani Williams**  
Master of Science in Computer Science (Artificial Intelligence)  
Troy University

---

## Research Information

**Course:** CS 6625 Specialized Study  
**Instructor:** Dr. Long Ma  
**Term:** Term 5, 2026  
**Status:** Completed

---

## Abstract

This study compares rule based, supervised, and unsupervised approaches for anomaly detection using HDFS (Hadoop Distributed File System) system logs. Four engineered feature sets were evaluated using a Statistical Baseline, Logistic Regression, Random Forest, and Isolation Forest. Model performance was measured using Accuracy, Precision, Recall, and F1 Score to determine how detection method and feature representation influence anomaly detection performance. The experimental results demonstrate that supervised machine learning approaches consistently outperformed both the statistical baseline and the unsupervised Isolation Forest model, with Random Forest achieving the strongest overall performance.

---

## Overview

This repository contains the complete implementation, datasets, notebooks, experimental results, and research paper for the comparative study.

Each notebook represents one stage of the experimental workflow, allowing the study to be reproduced from raw data preparation through final model evaluation and performance comparison.

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

These files provide the feature matrix and ground truth labels used to evaluate rule based, supervised, and unsupervised anomaly detection approaches.

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
- **results/** contains exported evaluation metrics, trained model outputs, and comparison results.
- **paper/** contains the final research manuscript.

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

## Experimental Results

The study evaluates each anomaly detection approach using the following performance metrics:

- Accuracy
- Precision
- Recall
- F1 Score

The Statistical Baseline provides a rule based benchmark, while Logistic Regression, Random Forest, and Isolation Forest are evaluated using the same engineered feature sets to enable direct performance comparisons.

Among the evaluated approaches, Random Forest achieved the highest overall performance, followed by Logistic Regression. The Statistical Baseline provided an interpretable benchmark, while Isolation Forest produced the weakest overall performance on the HDFS dataset.

---

## Repository Contents

This repository includes:

- Complete experimental notebooks
- Feature engineering pipeline
- Statistical Baseline implementation
- Logistic Regression implementation
- Random Forest implementation
- Isolation Forest implementation
- Comparative performance evaluation
- Final IEEE research paper
- Reproducible dataset archive reference

---

## References

1. Wei Xu, Ling Huang, Armando Fox, David Patterson, Michael Jordan. *Detecting Large Scale System Problems by Mining Console Logs.* Proceedings of the 22nd ACM Symposium on Operating Systems Principles (SOSP), 2009.

2. Jieming Zhu, Shilin He, Pinjia He, Jinyang Liu, Michael R. Lyu. *LogHub: A Large Collection of System Log Datasets for AI-driven Log Analytics.* IEEE Transactions on Software Engineering, 2023.

3. M. Du, F. Li, G. Zheng, and V. Srikumar. *DeepLog: Anomaly Detection and Diagnosis from System Logs through Deep Learning.* ACM CCS, 2017.

---

## Citation

If you use this repository in academic work, please cite the accompanying research paper.

---

## License

This repository is intended for academic research and educational purposes.

The HDFS dataset is distributed by the LogHub project and remains subject to its original licensing and usage terms.
