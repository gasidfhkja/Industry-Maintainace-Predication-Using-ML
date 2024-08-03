
# Problem statement
In today’s business environment, machines are crucial and must perform optimally over extended periods. Traditionally, corrective maintenance was used to address issues as they arose, but this approach can lead to significant downtime and higher labor costs.

Preventive maintenance aims to mitigate unplanned failures by addressing potential issues before they occur, though it can still be costly. Predictive maintenance improves on this by using real-time monitoring and prediction to address problems just in time, thus enhancing efficiency and reducing unexpected disruptions.

This project focuses on predictive maintenance, leveraging both supervised and unsupervised learning techniques. In supervised learning, the objectives include predicting the remaining useful life of machines and forecasting failures. In unsupervised learning, the goal is to detect anomalies in machine behavior. Python and its machine learning libraries are employed to develop these solutions. By implementing predictive maintenance, industries can minimize unexpected downtime and lower associated costs.

# Aims and objectives
The aim of this project is to propose machine learning solutions for predictive maintenance in responds to Industry 4.0. There are three tasks proposed:
* Anomaly detection: The model should be able to detect the anomalies within data.
* Remaining useful life prediction: The model should be able to predict the remaining useful life of a machine to help people be prepared for maintenance or replacement.
* Failure prediction: The model should be able to predict whether there will be a failure.

# Data 
There are two datasets used in this project as you can find in Datasets folder:
* [Bearings](https://github.com/Yi-Chen-Lin2019/Predictive-maintenance-with-machine-learning/tree/master/Datasets/bearings): Both anomaly detection and failure prediction use bearing dataset which is provided by [Case School of Engineering Bearing Data Center](https://engineering.case.edu/bearingdatacenter/download-data-file) and downloaded from [lestercardoz11’s public GitHub repository](https://github.com/lestercardoz11/fault-detection-for-predictive-maintenance-in-industry-4.0.git).
* [Battery](https://github.com/Yi-Chen-Lin2019/Predictive-maintenance-with-machine-learning/tree/master/Datasets/battery): Remaining useful life (RUL) task use battery dataset which is downloaded from [NASA](https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/#battery) and battery B0005 is chosen as study object.

# Solution 
This project adheres to the CRISP-DM methodology and employs both supervised and unsupervised learning algorithms to address specific tasks. Note that artificial neural networks (ANNs) are not included in this project.

For anomaly detection, the following algorithms are used:
- Local Outlier Factor (LOF)
- Elliptic Envelope
- Isolation Forest
- One-Class Support Vector Machine (SVM)

For predicting the remaining useful life of machines, the project utilizes:
- Support Vector Machine Regressor
- Tree-based Pipeline Optimization Tool (TPOT) for automated machine learning, with the best model selected and evaluated. Given the high dimensionality of the data, feature importance analysis is conducted to reduce the dataset's size, and a feature-reduced version is modeled to compare computational efficiency and results.

For failure prediction, the following classifiers are applied:
- Logistic Regression
- K-Nearest Neighbors Classifier
- C-Support Vector Classification with linear kernel
- C-Support Vector Classification with RBF kernel
- Gaussian Naive Bayes
- Decision Tree
- Random Forest Classifier

# Copyright To Raghav