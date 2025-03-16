# Concept Drift Detection in Metabolomics-based Predictions under Cold-Stress Conditions in Plants

This repository contains a framework for detecting concept drift in metabolomics data using machine learning models. The study focuses on metabolite concentrations and their relationship with relative growth rates at two different temperatures (6°C and 16°C). The project implements various regression models and concept drift detection methods to evaluate prediction stability over time.

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [How to Use](#how-to-use)
4. [Data Processing](#data-processing)
5. [Concept Drift Detection](#concept-drift-detection)
6. [Evaluation](#evaluation)

## Introduction
This project aims to detect concept drift in metabolite concentrations across different ecotypes of *Arabidopsis thaliana* under varying growth conditions. It consists of two main parts:
- Applying predictive regression models to metabolomic data.
- Detecting concept drift using these models to identify confounding factors affecting relative growth rate prediction.

## Installation
To set up the environment, install the required dependencies:
```bash
pip install -r requirements.txt
```

## How to Use
### Running on Google Colab
1. **Clone the Repository:**
```bash
!git clone <repository_url>
```
Replace `<repository_url>` with the actual GitHub link.

2. **Upload Data to Google Drive** and mount it in Colab:
```python
from google.colab import drive
drive.mount('/content/drive')
```

3. **Run the Notebook**
Execute the cells sequentially to preprocess data, train models, and detect concept drift.

## Data Processing
- Load and preprocess metabolomics data.
- Normalize and scale data using various scaling techniques.
- Train multiple regression models (Ridge, SVR, RF, DNN).

## Concept Drift Detection
- Implement **DDM (Drift Detection Method)** and **EDDM (Enhanced Drift Detection Method)**.
- Analyze drift effects on prediction stability.

## Evaluation
- Assess model accuracy, precision, and recall.
- Identify key confounding factors affecting metabolomics predictions.
---
**Datasets & Literature**:

> WEISZMANN, J. et al. Metabolome plasticity in 241 Arabidopsis thaliana accessions reveals evolutionary cold adaptation processes, 2023.

> Schwarzerova, Jana, et al. "An innovative perspective on metabolomics data analysis in biomedical research using concept drift detection." 2021 IEEE International Conference on Bioinformatics and Biomedicine (BIBM). IEEE, 2021.
 
>Schwarzerova, Jana, et al. "A revealed imperfection in concept drift correction in metabolomics modeling." International Conference on Information Technologies in Biomedicine. Cham: Springer International Publishing, 2022.


