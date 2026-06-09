# HDFS Dataset

This research utilizes the HDFS_v1 dataset for anomaly detection experiments.

Dataset Download:
https://www.kaggle.com/datasets/platform934/hdfs-log-dataset

Original Source:
https://github.com/logpai/loghub

Files Used:

* Event_occurrence_matrix.csv
* anomaly_label.csv
* Event_traces.csv
* HDFS.log_templates.csv

The dataset files are not stored in this repository due to file size limitations and because the dataset is publicly available from the sources above.

Dataset Description:

HDFS (Hadoop Distributed File System) is a distributed file storage system designed to run on commodity hardware.

The HDFS_v1 dataset was generated in a private cloud environment using benchmark workloads and manually labeled through handcrafted rules to identify anomalous behavior. Logs were sliced into traces according to block IDs, and each trace was assigned a ground-truth label of either normal or anomaly.

Citation:

Wei Xu, Ling Huang, Armando Fox, David Patterson, Michael Jordan. Detecting Large-Scale System Problems by Mining Console Logs. Proceedings of the 22nd ACM Symposium on Operating Systems Principles (SOSP), 2009.

Jieming Zhu, Shilin He, Pinjia He, Jinyang Liu, Michael R. Lyu. Loghub: A Large Collection of System Log Datasets for AI-driven Log Analytics. IEEE International Symposium on Software Reliability Engineering (ISSRE), 2023.

## Dataset Setup

Download the HDFS dataset from Kaggle:

https://www.kaggle.com/datasets/platform934/hdfs-log-dataset

Place the following files in:

data/processed/

- Event_occurrence_matrix.csv
- anomaly_label.csv
- Event_traces.csv
- HDFS.log_templates.csv
