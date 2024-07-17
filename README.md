# Collaborative Filtering Recommendation System

This project demonstrates the implementation of a collaborative filtering recommendation system using Google Dataproc and Apache Spark. The system processes user data to generate personalized recommendations.

## Table of Contents

1. [Introduction](#introduction)
2. [Design](#design)
3. [Implementation](#implementation)
4. [Test](#test)
5. [Enhancement Ideas](#enhancement-ideas)
6. [Conclusion](#conclusion)

## Introduction

This project aims to build a collaborative filtering recommendation system using Apache Spark on Google Dataproc. The goal is to process large datasets efficiently and provide accurate, personalized recommendations based on user interactions.

## Design

### Technologies Used

- **Google Dataproc**: Managed Spark and Hadoop service to handle data processing and analysis.
- **Apache Spark**: Distributed computing framework used for big data processing and machine learning.
- **Python**: Programming language used for scripting and implementing the recommendation algorithm.
- **Machine Learning**: Collaborative filtering technique to generate personalized recommendations based on user data.

## Implementation

### Setup Instructions

1. **Set Up a Dataproc Cluster**
   - Create a Dataproc cluster on Google Cloud Platform.

2. **SSH into the Dataproc Cluster**
   - Access the cluster using SSH from the Google Cloud Console.

3. **Install PySpark on the Cluster**
   - Verify PySpark installation using `pyspark --version`.

4. **Create and Upload Python Script**
   - Develop a Python script (`convert_data.py`) to preprocess data.
   - Upload your dataset (`u.data`) to the cluster.

5. **Run the Data Conversion Script**
   - Execute the script to prepare data for analysis.

6. **Install Apache Spark (if needed)**
   - Install Spark and its dependencies on your VM using the provided commands:
     ```bash
     sudo apt-get update
     sudo apt-get install default-jdk scala git -y
     wget https://dlcdn.apache.org/spark/spark-3.3.0/spark-3.3.0-bin-hadoop3.tgz
     tar -xzf spark-3.3.0-bin-hadoop3.tgz
     cd spark-3.3.0-bin-hadoop3
     ```

7. **Update and Run the Collaborative Filtering Script**
   - Modify and execute the recommendation script (`recommendation.py`) to generate recommendations.

## Test

- Validate the implementation by running the recommendation script and checking the output for accuracy.
- The system should provide a low Mean Squared Error (MSE) indicating the quality of recommendations.

## Enhancement Ideas

- Explore advanced machine learning techniques to improve recommendation accuracy.
- Scale the system for larger datasets and more complex models.
- Integrate additional features or data sources to enhance recommendations.

## Conclusion

The collaborative filtering recommendation system was successfully implemented using Google Dataproc and Apache Spark. The system efficiently processed large datasets and provided accurate, personalized recommendations. Future work includes enhancing the model and scaling the system for broader use.
