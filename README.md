

# Social Network Model


This paper establishes the user influence prediction model, and further divides the work roughly into data set acquisition, model building and experimental results evaluation. 

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
There are four parts in the document. Database establishment is in file named Weibo, which can be downloaded merely for web crawler. The other parts: process data, set up model and analysis are included in model.zip.


## Built With
- - -
The whole project is built with PyTorch 0.4.0.


### Database Setup
- - -
After downloading Weibo, the folder contains three parts: 
- parser : use web crawler to search required information on Weibo.
- writer : write the data in needed form.
- weibo ：contain all the raw information.

If you would like to choose other database, you could choose from:
* [Digg dataset](https://www.isi.edu/~lerman/downloads/digg2009.html)
* [Twitter dataset](https://snap.stanford.edu/data/higgs-twitter.html)
* [OAG dataset](https://www.openacademic.ai/oag/)
* [Weibo dataset](https://www.aminer.cn/influencelocality)


### Process Data
- - -
Process data to get the information specialize in social network, like features inluding
- deepwalk
- adjacency_matrix
- label
- vertex_feature


### Modified [Deepinf][1] Model
- - -
This document establishes the social network influence prediction model, divided into network embedding layer, instance regularization layer, input layer, graph convolution layer and output layer.


### Anaylysis
- - -
The document analysed and compared the results with LR,SVM and PSCN. 
The results will be collected and shown in table in four aspects:
- AUC(Area Under Curve) : Area under ROC curve with FPR as horizontal axis and TPR as vertical axis
- Prec(Precision)
- Rec(Recall)
- F1-value : the harmonic mean of accuracy and recall rate, which is jointly determined by Prec and Rec



### Bug / Feature Request
- - -
If you find a bug (the website couldn't handle the query and / or gave undesired results), kindly open an issue here by including your search query and the expected result.

If you'd like to request a new function, feel free to do so by opening an issue [here][2]. Please include sample queries and their corresponding results.




[1]:https://arxiv.org/abs/1807.05560
[2]:https://github.com/Greco79/bishe/issues


## License
MIT
