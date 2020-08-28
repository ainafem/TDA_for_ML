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

1. [Gudhi Tutorial](GudhiTutorial.ipynb)

It shows basic operations necessary to perform Topological Data Analysis. 

2. [Initial Exploration](TDA_Arrhythmia_Exploration.ipynb)

Contains the first exploration of the data that we performed. There are no exposable results here.

3. [Topological Data Analysis with distances](TDA_distances.ipynb)

Performs a more Machine Learning approach of the problem. We play with our dataset, landscape representations and several distances.

4. [Topological Data Analysis with Deep Learning](TDA_DeepLearning.ipynb)

Mixes the results of Topological Data Analysis with the power of Deep Learning. 

5. [Reconstruction of signals from Persistence Diagrams](mathematical_reconstruction.ipynb)

Proposes an algorithm to reconstruct signal functions from three different persistence diagrams. Compares such algorithm with a naive algorithm. Checks that the algorithm reconstructs piece-wise linear functions and applies the result to ECG heartbeats.

## Conclusions

In this master thesis, we give a comprehensible theoretical background for the study of Persistent Homology and, more precisely, the study of Topological Data Analysis. We give examples of computations and programs that can be applied with real world data. Moreover, we explore the possibility of the reconstruction of functions, a very recent problem (last papers are from 2020). In that sense, we give a new original algorithm that is able to reconstruct, up to piece-wise homotopy, piece-wise linear functions. 

Then, we apply Topological Data Analysis to a particular problem: classifying anomalies in ECG heartbeats. For that matter, we apply TDA as a exploratory tool of the data. Later on, we also use Persistent Homology as a feature extractor to enhance the Deep Learning capabilities. In that line, we propose a new data representation through Persistent Landscapes and we check that they contain important geometrical information. Moreover, we study the explainability properties that they have through the reconstruction of important landscapes that the network has selected. 

In summary, original contributions:
1. A different reconstruction algorithm for functions from three persistence diagrams.
2. An insightful vision of TDA as a tool to explore a dataset.
3. A new data representation using Persistence Landscapes as features to feed a neural network.
4. A new layer that automatically selects the more important landscapes.
5. Explanation and interpretation of the results through the reconstruction of the original signal using the selected landscapes by the network.
