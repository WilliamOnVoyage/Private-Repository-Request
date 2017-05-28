# Private-Repository-Summary
**A summary of my current projects and explanation**

Since my current projects contains confidential information, I cannot share them publicly. Yet I provide a list of each project's purpose, methods and techniques used, if you find anything interesting, please contact me for further discussion and collaboration.

## **Cooperative Projects**

**1. Understanding workflow data with deep learning**
|Python 3.5|
|----|
|![Build Status](https://travis-ci.com/WilliamOnVoyage/ActivityPrediction_TF.svg?token=mAvX7VnJxpyB9MUv3mSv&branch=master)|


We use deep learning based approach (specifically Recurrent and Convolutional Neural Network) to model workflow data in real-life, and understand how activities influence the future activities and other attributes.

**2. Process Progress Modeling and Understanding**

We use sensor data and machine learning algorithm to recognize real-life activities, and then perform classification and prediction on other attributes of the activities. E.g., the activities' execution forms the process, and we would like to know what is the current progress of process from the activities. We proposed a new system of Process Progress Estimation and Phase Detection to detect current phase and progress of the whole process. The estimation can predict the time left for the process based on observed activities and statistical distribution of activities/phases duration.

**3. Process Mining and Analysis**

In this project, we analyze the workflow both by data-driven techniques and by comparison to the expert model. 
Data-driven techniques: We use trace alignment method to align activities in workflow records so that common patterns of activities are captured. The common patterns are represented by the consensus sequence in the alignment. The higher frequency of an activity in one column indicates the activity is more likely to happen in such place. Though trace alignment deals with sequential data, the original algorithm does not support the attribute of duration. We proposed a Duration-Aware Alignment of Process Traces method to handle real-life workflow data with duration. To evaluate the alignment algorithm's performance, several metrics have been proposed, a summary of these metrics and some modifications are in our Trace Alignment Evaluation Methods.
Expert model techniques: The consistency of a workflow case and the expert model can be measured by conformance checking, which compares workflow data to a graph-based expert model and calculates the difference. The less difference indicates workflow data matches expert model more, vice versa. Though the expert model is predefined based on domain knowledge, which may be subjective and biased, the expert model based methods are necessary to guide other data-driven methods with its human labels.

## **Individual Projects**

**1. Game Performance Statistical Analysis**
|Python 3.5|
|----|
|![Build Status](https://travis-ci.com/WilliamOnVoyage/WOWS_stats.svg?token=mAvX7VnJxpyB9MUv3mSv&branch=master) |
Use deep learning method to analyze players' performance in an MMOTPS game World of Warships. Data acquired using public API provided by Wargaming.
Built modeling system based on Generative Adversarial Network and Reinforcement Learning methods, which models the adversarial procedure in game and calculates real-time prediction of the wining probability of both sides.

**2. Stock/Bioinformatics Data Analysis**
|Python 3.5|
|----|
| ![Build Status](https://travis-ci.com/WilliamOnVoyage/XDBIO_Master.svg?token=mAvX7VnJxpyB9MUv3mSv&branch=master)|
Use machine learning and other basic statistical methods to analyze stock prices and bioinformatics data. The algorithms are developed based on Weka library in Java, and the software GUI is built on Java.Swingx.
Applied auto sampling method on sensor data with statistical range from historical sample data, replaced human sampling procedure.
