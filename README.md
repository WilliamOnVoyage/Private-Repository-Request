Private-Repository-Summary
===

**A summary of my current projects and explanation**

Since my current projects contain confidential data and corresponding model structure, I cannot share them publicly. Yet I provide a list of each project's purpose, methods and techniques used, if you find anything interesting, please contact me for further discussion and collaboration.

More detailed theoretical explanation on [my projects website](https://sites.google.com/view/moliangzh/projects)

## Individual Projects

### [1. Game Performance Statistical Analysis (**Public now**)](https://williamonvoyage.github.io/World-of-Warships-Stats-Analysis/)  
[![Build Status](https://travis-ci.org/WilliamOnVoyage/World-of-Warships-Stats-Analysis.svg?branch=master)](https://travis-ci.org/WilliamOnVoyage/World-of-Warships-Stats-Analysis) [![Test Coverage](https://codeclimate.com/github/WilliamOnVoyage/World-of-Warships-Stats-Analysis/badges/coverage.svg)](https://codeclimate.com/github/WilliamOnVoyage/World-of-Warships-Stats-Analysis/coverage) [![Code Health](https://landscape.io/github/WilliamOnVoyage/World-of-Warships-Stats-Analysis/master/landscape.svg?style=flat)](https://landscape.io/github/WilliamOnVoyage/World-of-Warships-Stats-Analysis/master)
[![Pythonversion](https://img.shields.io/badge/python-3.5-blue.svg)](https://sourceforge.net/projects/winpython/files/WinPython_3.5/3.5.2.3/) [![MySQL](https://img.shields.io/badge/mysql-5.5-blue.svg)](https://dev.mysql.com/downloads/windows/installer/5.5.html) [![MongoDB](https://img.shields.io/badge/mongo-3.4-blue.svg)](https://docs.mongodb.com/manual/release-notes/3.4/?_ga=2.148716407.1370168894.1503081314-630273995.1503081314) [![Tensorflow](https://img.shields.io/badge/tensorflow-1.0.1-blue.svg)](https://github.com/tensorflow/tensorflow/tree/r1.0)

Use deep learning method to analyze players' performance in an MMOTPS game World of Warships. Data acquired using public API provided by Wargaming. Built modeling system based on Generative Adversarial Network and Reinforcement Learning methods, which models the adversarial procedure in game and calculates real-time prediction of the wining probability of both sides.

---------------------------

### 2. Stock/Bioinformatics Data Analysis  
![Build Status](https://travis-ci.com/WilliamOnVoyage/XDBIO_Master.svg?token=mAvX7VnJxpyB9MUv3mSv&branch=master) [![JavaVersion](https://img.shields.io/badge/java-8.0-blue.svg)](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) [![Code Health](https://landscape.io/github/WilliamOnVoyage/XDBIO_Master/master/landscape.svg?style=flat&badge_auth_token=d93c6fcebdf2479295bb05dc33fe44c3)](https://landscape.io/github/WilliamOnVoyage/XDBIO_Master/master)

Use machine learning and other basic statistical methods to analyze stock prices and bioinformatics data. The algorithms are developed based on Weka library in Java, and the software GUI is built on Java.Swingx.
Applied auto sampling method on sensor data with statistical range from historical sample data, replaced human sampling procedure.

## Cooperative Projects
### 1. Understanding workflow data with deep learning 
[![Build Status](https://travis-ci.com/WilliamOnVoyage/ActivityPrediction_TF.svg?token=mAvX7VnJxpyB9MUv3mSv&branch=master)](https://travis-ci.com/WilliamOnVoyage/ActivityPrediction_TF) [![Pythonversion](https://img.shields.io/badge/python-3.5-blue.svg)](https://sourceforge.net/projects/winpython/files/WinPython_3.5/3.5.2.3/) [![Code Health](https://landscape.io/github/WilliamOnVoyage/ActivityPrediction_TF/master/landscape.svg?style=flat&badge_auth_token=d93c6fcebdf2479295bb05dc33fe44c3)](https://landscape.io/github/WilliamOnVoyage/ActivityPrediction_TF/master)

We use deep learning based approach (specifically CNN and LSTM) to model workflow data in real-life, and understand how activities influence the future activities and other attributes.
The model aims at predicting activities' combination of the next time instance given the previous activities. The activities are coded as binary sequences over time, however, during the training phase for LSTM, binary representation of activities met imbalance data problem and caused the LSTM overfitting to the idle activities. We proposed a data pre-processing method to solve this problem.
The trained LSTM model is able to predict next time activity combination as a vector and reaches 70% accuracy.

--------------------------

### 2. Process Progress Modeling and Understanding

We use sensor data and machine learning algorithm to recognize real-life activities, and then perform classification and prediction on other attributes of the activities. E.g., the activities' execution forms the process, and we would like to know what is the current progress of process from the activities. We proposed a new system of Process Progress Estimation and Phase Detection to detect current phase and progress of the whole process. The estimation can predict the time left for the process based on observed activities and statistical distribution of activities/phases duration.

---------------------------
### 3. Process Mining and Analysis

In this project, we analyze the workflow both by data-driven techniques and by comparison to the expert model. 
Data-driven techniques: We use trace alignment method to align activities in workflow records so that common patterns of activities are captured. The common patterns are represented by the consensus sequence in the alignment. The higher frequency of an activity in one column indicates the activity is more likely to happen in such place. Though trace alignment deals with sequential data, the original algorithm does not support the attribute of duration. We proposed a Duration-Aware Alignment of Process Traces method to handle real-life workflow data with duration. To evaluate the alignment algorithm's performance, several metrics have been proposed, a summary of these metrics and some modifications are in our Trace Alignment Evaluation Methods.
Expert model techniques: The consistency of a workflow case and the expert model can be measured by conformance checking, which compares workflow data to a graph-based expert model and calculates the difference. The less difference indicates workflow data matches expert model more, vice versa. Though the expert model is predefined based on domain knowledge, which may be subjective and biased, the expert model based methods are necessary to guide other data-driven methods with its human labels.
