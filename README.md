# Predict-APS-System-Failures-in-Scania-Trucks

## Advanced Data Science Capstone Project - IBM Coursera 

## Data Set

The data set consists of data collected from heavy Scania trucks in everyday usage. The system in focus is the Air Pressure system (APS) which generates pressurized air that is utilized in various functions in a truck, such as braking and gear changes. The data sets' positive class consists of component failures for a specific component of the APS system. The negative class consists of trucks with failures for components not related to the APS. The data consists of a subset of all available data, selected by experts. The training set contains 60000 examples in total in which 59000 belong to the negative class and 1000 positive class. The test set contains 16000 examples. There are 171 attributes per record. It was imported from the UCI ML Repository https://archive.ics.uci.edu/ml/datasets/APS+Failure+at+Scania+Trucks

## Use Case

**Create a model that accurately predict APS system failures in Scania Trucks and reduce the cost of failures.**

Total cost = Cost_1 * Number of Instances of False Positive Cases + Cost_2 * Number of Instances of False Negative Cases

Cost_1 = $10 (The cost that an unnecessary check needs to be done by an mechanic at an workshop)

Cost_2 = $ 500 (The cost of missing a faulty truck, which may cause a breakdown)

## Architectural Choices
1. IBM watson Juyter Notebook
2. IBM watson Apache Spark
3. Pandas
4. matplotlib
5. seaborn
6. Apache Spark ML
7. scikit learn
8. Keras
9. scikit plot

## Solution Model
I have tried with different machine learning and deep learning models to find out the model that accurately predict the APS system failures and reduce the cost of failures. Almost all model were giving more than 98% accuracy. But cost of models were high. But logistic regression classifier with Apache Spark ML library was able to achieve zero cost. So selected logistic regression classifier with Apache Spark ML library as the solution model.

Please view the project on [IBM Watson Jupyter Notebook](https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/4874578f-dfcd-4b00-ae09-1d29478a0fdf/view?access_token=b130995737958132804bbaa2fb67ca663847651d41e2a809aa161ae54c386a4e)
