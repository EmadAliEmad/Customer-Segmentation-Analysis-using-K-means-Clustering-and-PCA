# Customer Segmentation Analysis using K-means Clustering and PCA

## Project Description

This project demonstrates customer segmentation using unsupervised machine learning techniques, specifically K-means clustering and Principal Component Analysis (PCA). The analysis aims to group customers based on their purchasing behavior and demographic data. The dataset used is created for learning purposes, mimicking the kind of data found in a supermarket mall with membership cards.

The project provides insights into:

1.  **How to achieve customer segmentation using the K-means algorithm.**
2.  **Identifying customer groups based on their behavior and purchasing data.**
3.  **Understanding how marketing strategies can be tailored to specific groups**.

## Files in this Repository

*   **`IEEE Session 7 Task K_mean, PCA.ipynb`**: Jupyter Notebook containing the code for data analysis, model building, and visualization.
*   **`Mail_Customers.csv`**: Dataset containing customer information.
*   **`README.md`**: This file, providing an overview of the project.

## How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/EmadAliEmad/Customer-Segmentation-Analysis-using-K-means-Clustering-and-PCA.git
    cd Customer-Segmentation-Analysis-using-K-means-Clustering-and-PCA
    ```

2.  **Ensure You Have Python Installed:** This project requires Python 3.6 or higher.

3.  **Install Required Libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

4.  **Open and Run the Jupyter Notebook:**
    *   Open the `IEEE Session 7 Task K_mean, PCA.ipynb` file using Jupyter Notebook or JupyterLab.
    *   Execute the cells in order to run the analysis. The notebook provides visualizations for each step of the analysis, such as Heatmap, histograms, elbow curve, and the final clusters, along with the numerical values for the cluster centers.

## Project Logic Overview

The Jupyter Notebook `IEEE Session 7 Task K_mean, PCA.ipynb` contains the following key steps:

1.  **Import Libraries:** Imports the necessary libraries for data manipulation, visualization, and machine learning.
2.  **Load the Dataset:** Loads the `Mall_Customers.csv` file into a Pandas DataFrame.
3.  **Explore the Dataset:**
    *   Displays information about the dataset's structure using `df.info()`.
    *   Provides descriptive statistics for numerical columns using `df.describe()`.
    *   Checks for missing values using `df.isnull().sum()`.
4.  **Data Preprocessing:**
    *   Scales numerical features (Age, Annual Income, Spending Score) using `StandardScaler`.
5. **Data Visualization**:
     *   Generates a correlation heatmap to understand relationships between features.
     *   Generates a scatter plot for `Annual Income (k$)` and `Spending Score (1-100)` and a histogram for `Age`.
6.  **Dimensionality Reduction (PCA):**
    *   Applies PCA to reduce the dimensionality of the scaled data to 2 components.
7.  **K-means Clustering:**
    *   Uses the Elbow method to identify the optimal number of clusters.
    *   Applies K-means clustering to group customers based on PCA reduced data.
    *   Visualizes the customer clusters in 2D space, along with their centroids.
   *   Prints the number of clusters and their respective centers.

## Data Source

The data for this project is stored in the `Mall_Customers.csv` file. It is a dataset that contains information about customers in a supermarket mall, like customerID, gender, age, annual income, and spending score.

## Dependencies

*   **Python 3.6 or higher**
*   **Pandas:** For data manipulation and analysis.
*   **NumPy:** For numerical calculations.
*   **Matplotlib:** For data visualization.
*   **Seaborn:** For statistical data visualization.
*   **Scikit-learn:** For machine learning algorithms and preprocessing.

## Potential Improvements

*   Explore different clustering algorithms and evaluate their performance.
*   Implement different scaling and normalization techniques.
*   Add a section that analyzes each cluster, identifying their key characteristics.
*   Add more comments in the `IEEE Session 7 Task K_mean, PCA.ipynb` file.
*   Perform a hyper-parameter optimization for PCA and K-means algorithms.

## License

This project is open-source and available for use under the MIT License.

## Author

*   **Emad Ali Emad**
    [GitHub Profile](https://github.com/EmadAliEmad)
