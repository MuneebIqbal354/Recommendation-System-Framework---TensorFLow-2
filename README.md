# Recommendation System Framework - TensorFLow 2

![TensorFlow](https://img.shields.io/badge/TensorFlow-2.3.2-orange.svg) ![Python](https://img.shields.io/badge/Python-3.8-blue.svg) ![Status](https://img.shields.io/badge/Status-Active-green.svg)

This repository hosts an actively developed collection of recommendation system algorithms implemented using **TensorFlow 2**. The project aims to provide a comprehensive library of both traditional and deep learning-based models for research and development purposes.

## Supported Datasets

The models in this framework are tested against a variety of popular datasets:

* **MovieLens:** Versions 100k, 1M, and 20M.
* **Last.fm:** Music listening data.
* **Book-Crossing:** Book ratings and user data.
* **Satori:** Knowledge Graph data.

## Implemented Algorithms

This repository includes implementations for a wide range of algorithms, covering Collaborative Filtering, Factorization Machines, and Graph Neural Networks.



### Categories:
* **Collaborative Filtering:** UserCF (User-based), ItemCF (Item-based).
* **Latent Factor & Linear Models:** LFM (Latent Factor Model), SLIM (Sparse Linear Method), FM (Factorization Machines).
* **Neural Collaborative Filtering:** GMF (Generalized Matrix Factorization), MLP (Multi-Layer Perceptron), NeuMF (Neural Matrix Factorization).
* **Deep Learning:** DeepFM.
* **Knowledge Graph & Network:** MKR (Multi-task Feature Learning for Knowledge Graph Enhanced Recommendation), RippleNet, KGCN (Knowledge Graph Convolutional Networks).

## Evaluation Metrics

Performance is evaluated using standard industry metrics:

* **CTR Prediction:** AUC (Area Under Curve) and F1-Score.
* **Top-K Recommendation:** Precision and Recall.

## Requirements

Ensure your environment meets the following specifications:

* **Python:** 3.8
* **TensorFlow:** 2.3.2

## Getting Started

### 1. Installation & Setup
It is recommended to open the parent directory of this file as a project in **PyCharm**.

Set up your interpreter to use **Python 3.8** and install the required dependencies:

```bash
pip install tensorflow==2.3.2
```

### 2. Dataset Configuration
> **Note:** Due to file size limitations, the **MovieLens-20m** dataset is not included in this repository.

If you require the 20M dataset:
1.  Download it manually from [GroupLens](https://grouplens.org/datasets/movielens/20m/).
2.  Extract the contents.
3.  Place the `ml-20m` folder into the following directory:
    `Recommender_System/data/ds`

### 3. Running the Models
Navigate to the specific algorithm folder you wish to test and execute the `main.py` script. 

**Example:**
```bash
cd Recommender_System/algorithm/[ALGORITHM_NAME]
python main.py
```

