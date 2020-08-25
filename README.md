# Topological Data Analysis for Machine Learning
## Introduction
The study of Persistent Homology is a fairly new subject that started in the decade of the 1990s. Until 2005, the main focus of the study was to find optimal algorithms to compute Homology Groups. From 2005 forward, the study shifted towards the more abstract algebraic properties of the subject. It was not until 2015, when Persistence Landscapes were introduced, that the subject of Topological Data Analysis was born. TDA tries to find significative relations and information about data using some homological features.

In this master thesis, we study the possible applications of Topological Data Analysis to the field of Machine Learning and, particularly, Deep Learning. We follow a methodological approach: rather than solving a specific problem, we investigate the possible usages in a general context. For that reason, we apply Topological Data Analysis to the following:
1. Analysis of a training data set: we analyze the possible underlying sets and check if the proposed classes are respected by their homological features.
2. Classification through homological features: we apply classic Machine Learning techniques and try to classify samples solely based on their homological features.
3. Feature extracting: we use Persistent Homology as a tool to extract features that will be fed to a Neural Network. In fact, we propose a new representation -through Persistence Landscapes- in contraposition to the ones commonly used.
4. Interpretability of the results: we propose a new layer for Deep Learning that works with our new representation of the Data, that is capable of selecting the important features. Moreover, using Persistent Homology, we reconstruct the signal input from the selected features to give an explanation to what a Neural Network is selecting.

## Notebooks
The following notebooks have been produced as a result of this thesis. Note that all notebooks are ready to be executed in Google Colab, and as such, they have implemented a snippet of cod that downloads Gudhi and the dataset from Kaggle. If the code has to be executed in a local computer, one will need the Gudhi library and Keras. 

1. GudhiTutorial.ipynb

It shows basic operations necessary to perform Topological Data Analysis. 

2. TDA_Arrhythmia_Exploration.ipynb

Contains the first exploration of the data that we performed. There are no exposable results here.

3. TDA_distances.ipynb

Performs a more Machine Learning approach of the problem. We play with our dataset, landscape representations and several distances.

4. TDA_DeepLearning.ipynb

Mixes the results of Topological Data Analysis with the power of Deep Learning. 
