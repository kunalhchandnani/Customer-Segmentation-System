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

![Distribution of Balance](https://github.com/user-attachments/assets/d7941f63-f13d-466e-b819-a884523157a2)

![Balance vs Purchases Colored by Credit Limit](https://github.com/user-attachments/assets/a5c6ec64-5ff3-4cbf-800d-87aadbf1bb25)

![Correlation Matrix](https://github.com/user-attachments/assets/99260041-927c-4d72-aaa7-07dd1f7f7b56)

![Pairwise Relationships](https://github.com/user-attachments/assets/cf0076fe-a250-4525-bbad-b9693f8dd724)

![Boxplot of Balance by Tenure](https://github.com/user-attachments/assets/589bf9f6-ef38-4ebc-bba6-d588d46766de)

![Purchases vs Payments Segmentation by Tenure](https://github.com/user-attachments/assets/f6d90d34-8e7c-42da-af1d-2ce767633108)

![Purchases Frequency](https://github.com/user-attachments/assets/6f549354-4fb7-4b73-94d1-de7dfb252ed6)

![Payment Purchases 3D Plot](https://github.com/user-attachments/assets/424eb77f-60c1-4678-b9de-2b8758b5cb38)

![Purchase Frequency](https://github.com/user-attachments/assets/229208bc-96b7-4f3b-bc66-c1aede3dc22f)

![Purchase Categories Sunburst Chart](https://github.com/user-attachments/assets/b704e4df-40d6-4222-bde4-a5b913e3a427)

![Animate Bubble Chart for Cash Advance](https://github.com/user-attachments/assets/ef6dfeab-81eb-4de6-a912-2c22685e7b98)

![Purchases](https://github.com/user-attachments/assets/50ec2643-0153-4974-ae08-79a60d1a643c)

![Variance Ratio](https://github.com/user-attachments/assets/0768e9bd-acdf-4070-853f-07e5afd9fed8)

![Inertia](https://github.com/user-attachments/assets/ec8b7e6c-8c6f-4ff6-8dba-983c5012fb7e)

![Clusters Plot](https://github.com/user-attachments/assets/74f59269-3e67-4648-a995-1ae3d040e5d9)
















