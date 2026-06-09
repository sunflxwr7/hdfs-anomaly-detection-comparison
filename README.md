# Comparing Rule-Based, Supervised, and Unsupervised Approaches for Anomaly Detection in System Logs

## Author

**Tamani Williams**  
Master of Science in Computer Science (Artificial Intelligence)  
Troy University

## Research Information

**Course:** CS 6625 Specialized Study  
**Instructor:** Dr. Long Ma  
**Term:** Term 5, 2026  
**Status:** In Progress

## Abstract

This research investigates the effectiveness of traditional rule-based monitoring compared to supervised and unsupervised machine learning approaches for anomaly detection in distributed system logs. Using the HDFS (Hadoop Distributed File System) dataset, the study evaluates Rule-Based Detection, Logistic Regression, Random Forest, and Isolation Forest models. Performance is measured using accuracy, precision, recall, and F1 score to determine whether machine learning approaches can improve anomaly detection performance over static threshold-based methods.

## Overview

This repository contains the code, datasets, experiments, and research artifacts associated with this study.

## Dataset

This study utilizes the HDFS_v1 dataset, a benchmark dataset widely used in anomaly detection research for distributed systems.

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

These files provide the feature matrix and ground-truth labels used for evaluating rule-based, supervised, and unsupervised anomaly detection approaches.

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

* **data/** contains dataset references and supporting documentation.
* **notebooks/** contains exploratory analysis and experimentation notebooks.
* **src/** contains Python scripts used throughout the study.
* **results/** contains model outputs, evaluation metrics, and visualizations.
* **paper/** contains research planning documents and manuscript materials.

```
```

## Project Status

**Current Phase:** Data Acquisition and Experiment Setup

### Completed

* Research topic approved
* Project plan approved
* HDFS_v1 dataset obtained and validated
* Public dataset archive created
* GitHub repository established

### In Progress

* Data exploration
* Experimental environment setup
* Reproducibility documentation

### Upcoming

* Statistical threshold development
* Logistic Regression implementation
* Random Forest implementation
* Isolation Forest implementation
* Model evaluation and comparison

```
```

## References

1. Wei Xu, Ling Huang, Armando Fox, David Patterson, Michael Jordan. *Detecting Large-Scale System Problems by Mining Console Logs.* Proceedings of the 22nd ACM Symposium on Operating Systems Principles (SOSP), 2009.

2. Jieming Zhu, Shilin He, Pinjia He, Jinyang Liu, Michael R. Lyu. *LogHub: A Large Collection of System Log Datasets for AI-driven Log Analytics.* IEEE International Symposium on Software Reliability Engineering (ISSRE), 2023.

3. Zhihan Jiang, Jinyang Liu, Junjie Huang, Yichen Li, Yintong Huo, Jiazhen Gu, Zhuangbin Chen, Jieming Zhu, Michael R. Lyu. *A Large-scale Evaluation for Log Parsing Techniques: How Far are We?* ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA), 2024.

```
```
