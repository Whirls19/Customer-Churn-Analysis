# Customer Churn Analysis

## 📊 Project Overview

This project performs an in-depth Exploratory Data Analysis (EDA) on a customer churn dataset from a telecommunications company. The primary goal is to identify the key factors that contribute to customer churn. By understanding these drivers, businesses can develop targeted strategies to improve customer retention.

The analysis explores customer demographics, account information, and the services they use to uncover patterns and insights related to churn.

-----

## Dataset

The dataset contains information about telecom customers, including:

  * **Customer Demographics**: Gender, Senior Citizen status, Partner, and Dependents.
  * **Account Information**: Tenure (how long they've been a customer), Contract type, Payment Method, and Paperless Billing.
  * **Services Subscribed**: Phone Service, Multiple Lines, Internet Service (DSL, Fiber Optic), Online Security, Online Backup, Device Protection, Tech Support, Streaming TV, and Streaming Movies.
  * **Charges**: Monthly Charges and Total Charges.
  * **Target Variable**: Churn (Yes/No).

-----

## ⚙️ Technologies Used

  * **Python**: Core language for analysis.
  * **Pandas**: For data manipulation and cleaning.
  * **NumPy**: For numerical operations.
  * **Matplotlib & Seaborn**: For data visualization.
  * **Jupyter Notebook**: For interactive analysis and documentation.

-----

## Key Findings from the Analysis

### Data Cleaning and Preprocessing

  * The `TotalCharges` column had blank spaces for customers with zero tenure, which were replaced with `0` and the column type was converted to float.
  * The `SeniorCitizen` column, originally encoded as `0` and `1`, was mapped to `No` and `Yes` for better readability in visualizations.

### Overall Churn Rate

The dataset is imbalanced, with a churn rate of approximately **26.5%**. This means about one in four customers has left the service.

### Key Factors Influencing Churn

#### 1\. Contract Type

**Month-to-month contracts** have a significantly higher churn rate compared to one-year or two-year contracts. This is the strongest predictor of churn. Customers on longer contracts are more loyal.

#### 2\. Tenure

Customers with **low tenure** (especially those in their first few months) are far more likely to churn. Customer loyalty increases significantly with the length of service.

#### 3\. Internet Service

Customers with **Fiber optic** internet service have a much higher churn rate than those with DSL. Customers with no internet service have a very low churn rate.

#### 4\. Additional Services

Customers **without** value-added services like **Online Security**, **Online Backup**, **Device Protection**, and especially **Tech Support** are much more likely to churn. Tech support, in particular, appears to be a critical factor in customer retention.

#### 5\. Payment Method

Customers who pay by **Electronic check** exhibit the highest churn rate among all payment methods.

#### 6\. Demographics

**Senior Citizens** have a churn rate almost double that of non-seniors, making them a high-risk group.

-----

## 📈 Visualizations

The analysis relies on a variety of plots to uncover insights, including:

  * **Pie Charts**: To show the overall churn distribution.
  * **Count Plots**: To compare churn across categorical features like Gender, Contract, and Payment Method.
  * **Histograms**: To visualize the relationship between customer tenure and churn.
  * **Stacked Bar Charts**: To analyze the percentage of churn within different customer segments (e.g., Senior Citizens).

-----

## 🚀 How to Run this Project

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/customer-churn-analysis.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd customer-churn-analysis
    ```
3.  **Install the required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn jupyter
    ```
4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
5.  Open `ChurnDataAnalysis.ipynb` to view and run the analysis.

-----

## Conclusion

The analysis reveals several critical factors driving customer churn. The most influential predictors are short tenure, month-to-month contracts, fiber optic internet service, and the absence of key add-on services like tech support and online security. These insights can help the company focus its retention efforts on high-risk customer segments and improve service offerings to reduce churn.
