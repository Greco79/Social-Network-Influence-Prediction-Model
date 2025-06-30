

# Social Network Influence Prediction Model


This project builds a user influence prediction model within a social network environment. The workflow includes:

1. Dataset acquisition

2. Model construction

3. Experimental evaluation 

Table of content
- [Social Network Model](#social-network-model)
  - [Usage](#usage)
  - [Built With](#built-with)
    - [Database Setup](#database-setup)
    - [Process Data](#process-data)
    - [Modified Deepinf Model](#modified-deepinf-model)
    - [Anaylysis](#anaylysis)
    - [Bug / Feature Request](#bug--feature-request)
  - [License](#license)


## Usage
- - -
The project consists of four core components:

- The database setup is located in the Weibo folder and is intended for web crawling.

- The remaining parts—data preprocessing, model training, and result analysis—are provided in model.zip.


## Built With
- - -
The whole project is built with PyTorch 0.4.0.


### Database Setup
- - -
After downloading the Weibo dataset, the folder includes:
- parser/ : Web crawler scripts for collecting information from Weibo
- writer/ : Data transformation scripts for formatting
- weibo/ ：Raw collected data

Alternative public datasets you can experiment with:
* [Digg dataset](https://www.isi.edu/~lerman/downloads/digg2009.html)
* [Twitter dataset](https://snap.stanford.edu/data/higgs-twitter.html)
* [OAG dataset](https://www.openacademic.ai/oag/)
* [Weibo dataset](https://www.aminer.cn/influencelocality)


### Data Processing
- - -
Processed data includes key features for social network analysis:

- deepwalk — Node embeddings

- adjacency_matrix — Graph structure

- label — Influence labels for supervised learning

- vertex_feature — Additional node-level attributes


### Modified DeepInf Model
- - -
The influence prediction model follows a deep graph-based architecture consisting of:

- Network Embedding Layer

- Instance Regularization Layer

- Input Layer

- Graph Convolution Layer

- Output Layer

This architecture is a modified implementation of the DeepInf model.


### Anaylysis
- - -
Model performance is evaluated against classic baselines including Logistic Regression (LR), SVM, and PSCN.
Evaluation metrics include:

- AUC (Area Under Curve) – ROC curve performance

- Precision (Prec) – True positive rate among predicted positives

- Recall (Rec) – True positive rate among actual positives

- F1-Score – Harmonic mean of precision and recall

All results are organized into tables for comparison.



### Bug / Feature Request
- - -
If you find a bug (the website couldn't handle the query and / or gave undesired results), kindly open an issue here by including your search query and the expected result.

If you'd like to request a new function, feel free to do so by opening an issue [here][2]. Please include sample queries and their corresponding results.




[1]:https://arxiv.org/abs/1807.05560
[2]:https://github.com/Greco79/bishe/issues


## License
MIT
