# MallCustomerSegmentation

## Dataset

The dataset Mall_Customers.csv contains the following features:

*   *CustomerID:* Unique identifier for each customer.
*   *Gender:* Gender of the customer.
*   *Age:* Age of the customer.
*   *Annual Income (k$):* Annual income of the customer in thousands of dollars.
*   *Spending Score (1-100):* Score assigned by the mall based on customer spending behavior.

## Methodology

1.  *Data Loading and Exploration:*
    *   The dataset is loaded using pandas.
    *   Initial data exploration is performed to understand the structure and characteristics of the data.

2.  *Feature Selection:*
    *   The "Annual Income (k$)" and "Spending Score (1-100)" columns are selected as features for clustering.

3.  *K-Means Clustering:*
    *   The K-Means algorithm is used to cluster the customers into distinct groups.
    *   The optimal number of clusters is determined using the Elbow Method.
    *   The K-Means model is trained on the selected features.

4.  *Cluster Visualization:*
    *   The clusters are visualized using scatter plots, with different colors representing different clusters.
    *   Cluster centers (centroids) are also plotted.

5.  *Streamlit App:*
    *   An interactive Streamlit app is created to allow users to input custom annual income and spending score values.
    *   The app predicts the cluster to which a customer with the given input belongs.
    *   The app also displays a visualization of the clusters with the user's input highlighted.

6.  *Model Saving:*
    *   The trained K-Means model is saved as a pickle file for later use.

## Usage

1.  *Install the required dependencies:*

    
    pip install pandas scikit-learn matplotlib streamlit
    

2.  *Run the Streamlit app:*

    
    streamlit run Mall_Customer_Segmentation_app.py
    

3.  *Access the app in your browser:*

    *   The app will open in your default web browser. If it doesn't, you can usually find the URL in the terminal where you ran the command.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests.
