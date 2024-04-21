# Anomaly Detection using Negative Selection Algorithms

## Introduction
This project focuses on using the Negative Selection Algorithm for two main tasks:
1. Language discrimination between English and other languages.
2. Intrusion detection for Unix processes.

Each task is documented with methodologies, parameter optimizations, and results including ROC curves and AUC metrics.

## Repository Structure
- `/language-discrimination`: Contains all files for the language discrimination task, including Jupyter notebooks and ROC plots.
- `/intrusion-detection`: Includes all necessary files for the intrusion detection task, such as data preprocessing scripts, anomaly detection scripts, and visualization tools.

## Tasks and Results
### 1. Language Discrimination
This task involved distinguishing English from other languages using the Negative Selection Algorithm. Key points:
- **Methodology**: Employed Negative Selection Algorithm to generate anomaly scores, followed by AUC calculation and ROC curve construction.
- **Parameters**: Used `n=10` and variable `r` from 1 to 9 to find optimal discrimination capabilities.
- **Results**: Achieved the best discrimination with an AUC peak at `r=3`, illustrating effective sensitivity and specificity balance.

### 2. Intrusion Detection for Unix Processes
Focused on detecting anomalous sequences within Unix system calls using the same algorithm.
- **Preprocessing**: Sequences were extracted and transformed into fixed-length chunks.
- **Evaluation**: Used ROC curves and AUC scores to evaluate model performance across different settings (`n=7`, `r={2,3,4}`).
- **Optimal Settings**: Found `r=3` to offer a robust balance between detection capabilities and computational efficiency.

## Visualizations
Link to plots and ROC curves that illustrate the findings:
- [Language Discrimination ROC Curves](https://github.com/andreas-pattichis/Anomaly-Detection-using-Negative-Selection-Algorithms/tree/main/NaCo%20-%20Assignment%203/1%20-%20Using%20the%20Negative%20Selection%20Algorithm/languages-comparison/plots)
- [Intrusion Detection ROC Curves](https://github.com/andreas-pattichis/Anomaly-Detection-using-Negative-Selection-Algorithms/tree/main/NaCo%20-%20Assignment%203/2%20-%20Intrusion%20Detection%20for%20Unix%20Processes/syscalls/snd-unm/plots)
