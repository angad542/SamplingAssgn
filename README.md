Sampling Assignment
Overview
This project focuses on applying various sampling techniques to a dataset and evaluating the performance of different machine learning models. The primary objective is to identify the best sampling approach for each model based on accuracy.

How to Run
Prerequisites
Ensure your system is set up with:

Python version 3.8 or higher.
The necessary Python libraries (details provided below).
Required Libraries
Install the required packages by running:
pip install pandas scikit-learn imbalanced-learn  
Dataset
The dataset for this project is titled Creditcard_data.csv and can be downloaded from the link below:
Download Dataset: [Creditcard_data.csv](https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv?raw=true)

Running the Script
Clone this repository or download the script file.
Make sure the dataset is available in the specified location (the script automatically handles fetching if needed).
Execute the script using the command:
python sampling_assignment.py  
Review the output to see which sampling techniques performed best for each machine learning model.
Project Details
Dataset Balancing
To handle class imbalances, the RandomOverSampler method from the imbalanced-learn library is used. This technique ensures the dataset is balanced before further processing.

Sampling Techniques
Five random samples are generated using the following formula to calculate sample size:
𝑛=𝑁/1+𝑁×𝑒^2
Here:
N represents the total population size.
e is the margin of error (default: 0.05).
Machine Learning Models
The script evaluates the performance of the following models:

Logistic Regression
Random Forest Classifier
Support Vector Classifier (SVC)
Gaussian Naive Bayes
K-Nearest Neighbors (KNN)
Evaluation Metrics
The models are evaluated based on their accuracy scores, and the sampling technique that yields the best performance for each model is identified.

Output
The script provides an analysis of the best sampling methods for each model. Example output:

Logistic Regression: Sampling1
Random Forest Classifier: Sampling3
Support Vector Classifier: Sampling4
Gaussian Naive Bayes: Sampling2
K-Nearest Neighbors: Sampling5
