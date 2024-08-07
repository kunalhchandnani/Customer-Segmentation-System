# Customer Segmentation System

---

## Table of Contents

1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Data Preprocessing](#data-preprocessing)
4. [Clustering with KMeans](#clustering-with-kmeans)
5. [Evaluation and Visualization](#evaluation-and-visualization)
6. [Web Application Deployment](#web-application-deployment)
7. [Usage](#usage)
8. [Results](#results)
9. [References](#references)
10. [License](#license)

---

## Introduction

Customer segmentation is a pivotal marketing strategy used to divide a customer base into distinct groups based on similar characteristics. This project employs machine learning techniques to segment customers, aiding businesses in tailoring their marketing efforts.

## Project Structure


- **Customer Data.csv**: The dataset containing customer information.
- **app.py**: The main Streamlit application file.
- **cluster_customer_data.csv**: The clustered customer data.
- **kmeans.pkl**: The saved KMeans model.
- **rc.pkl**: The saved recommendation model.
- **rc_model_2.sav**: Another saved model file.
- **requirements.txt**: List of dependencies.
- **testingone.ipynb**: Jupyter notebook for testing and analysis.

## Data Preprocessing

1. **Loading the Dataset**:
    - Read the customer data from `Customer Data.csv`.

2. **Cleaning the Data**:
    - Handle missing values and outliers.
    - Convert categorical variables into numerical ones using one-hot encoding.

3. **Feature Engineering**:
    - Create new features that might be useful for clustering.

4. **Scaling the Data**:
    - Normalize the data using `StandardScaler` to ensure all features contribute equally to the clustering.

## Clustering with KMeans

1. **Choosing the Number of Clusters**:
    - Use the Elbow method to determine the optimal number of clusters by plotting the Within-Cluster Sum of Squares (WCSS) against the number of clusters.

2. **Applying KMeans**:
    - Fit the KMeans model to the data.
    - Save the trained model using `joblib` for future use.

## Evaluation and Visualization

1. **Elbow Method**:
    - Plot the WCSS to find the "elbow point" which indicates the optimal number of clusters.

2. **Cluster Visualization**:
    - Use `plotly.express` to create 2D and 3D scatter plots of the clustered data.
    - Interpret the characteristics of each cluster.

## Web Application Deployment

1. **Streamlit Setup**:
    - Create a Streamlit app (`app.py`) to interact with the clustering results.
    - The app allows users to upload new data, visualize clusters, and download clustered data.

2. **Running the App**:
    - Deploy the app locally or on a cloud platform like Heroku or Streamlit Sharing.

## Usage

To use the Customer Segmentation System:

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/kunalhchandnani/Customer-Segmentation-System.git
    ```
2. **Navigate to the Project Directory**:
    ```sh
    cd Customer-Segmentation-System
    ```
3. **Install the Required Libraries**:
    ```sh
    pip install -r requirements.txt
    ```
4. **Run the Streamlit App**:
    ```sh
    streamlit run app.py
    ```

## Results

The system segments customers into distinct groups based on their purchasing behavior and demographic attributes. These insights enable businesses to customize their marketing strategies effectively.

