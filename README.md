# Customer-Churn-Analysis

# Project Overview

This project presents an end-to-end data science workflow focused on understanding and predicting customer churn for a simulated telecom or subscription-based business. The primary objective is to leverage data analysis and machine learning to identify customers at risk of churning and provide actionable strategies for retention.

The project workflow includes:

*   **Data Simulation:** Generating a realistic synthetic dataset representing customer behavior and demographics.
*   **Exploratory Data Analysis (EDA):** Visualizing and summarizing the dataset's main characteristics, identifying patterns, and understanding the distribution of churn.
*   **Statistical Analysis:** Performing hypothesis tests to determine the statistical significance of relationships between various features and customer churn.
*   **Predictive Modeling:** Building and evaluating machine learning models (Logistic Regression and Random Forest) to predict the probability of customer churn.
*   **Feature Importance Analysis:** Identifying the key factors that most influence churn predictions.
*   **Business Impact Quantification:** Estimating the potential financial savings achievable through targeted retention efforts.
*   **Actionable Recommendations:** Deriving strategic and operational recommendations based on the analysis and model insights.
*   **Deployment Preparation:** Creating functions and outputs to facilitate the implementation of the churn prediction model.

# Business Impact

Customer churn represents a significant loss of revenue for businesses. By effectively identifying and retaining customers at risk, a company can realize substantial cost savings and revenue protection. This analysis estimates that a **15% reduction in customer churn** for this business could lead to potential **annual revenue savings of approximately $[Your Estimated Annual Savings from Notebook]**.

# How to Run the Notebook

To explore and run the code yourself, follow these steps:

1.  **Clone the Repository:**
    Open your terminal or command prompt and run:
    ```bash
    git clone [Your GitHub Repository URL]
    cd [your-repository-name] # e.g., cd customer-churn-analysis-project
    ```

2.  **Create and Activate a Virtual Environment (Recommended):**
    Using a virtual environment helps manage project dependencies:
    ```bash
    python -m venv venv
    # On Windows:
    # .\venv\Scripts\activate
    # On macOS/Linux:
    # source venv/bin/activate
    ```

3.  **Install Dependencies:**
    Install all the necessary Python libraries listed in the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Open and Run the Notebook:**
    The dataset is generated within the notebook, so you don't need to download separate data files.
    *   **Using Google Colab:** Go to [https://colab.research.google.com/](https://colab.research.google.com/), click "File" -> "Upload notebook", and select the `Customer_Churn_Analysis.ipynb` file from your cloned repository. Once loaded, you can run all cells via `Runtime > Run all`.
    *   **Using Jupyter Notebook or JupyterLab:** Navigate to your repository folder in the terminal and run `jupyter notebook` or `jupyter lab`. Open the `Customer_Churn_Analysis.ipynb` file in your browser. You can run all cells sequentially.

# Repository Contents

*   `Customer_Churn_Analysis.ipynb`: The main Python notebook containing all code and analysis.
*   `requirements.txt`: Lists all Python libraries required to run the notebook.
*   `feature_importance.csv`: CSV file detailing the importance scores of features in the churn prediction model.
*   `model_predictions.csv`: CSV file containing the test set results including actual churn, predicted probabilities, and class predictions.
*   `high_risk_customers.csv`: CSV file identifying customers from the test set predicted to have a high churn probability.
*   `executive_summary.txt`: A non-technical summary of the project findings and recommendations suitable for business stakeholders.
*   `technical_summary.txt`: A more detailed summary of the methodology, data, and model for a technical audience.
*   `README.md`: This file, providing an overview and instructions.

# Key Findings

The analysis revealed several significant factors associated with higher churn rates:

*   **Contract Type:** Customers on **Month-to-month** contracts churn at a significantly higher rate compared to those with one-year or two-year contracts.
*   **Payment Method:** The **Electronic check** payment method shows a higher churn rate compared to automatic payment methods (Bank Transfer, Credit Card).
*   **Customer Service Calls:** A higher number of **Customer Service Calls** is strongly correlated with increased churn risk.
*   **Tenure and Charges:** Customers with shorter **Tenure** and higher **Monthly Charges** tend to churn more often. **Total Charges** also show a relationship with churn, though often linked to tenure and monthly charges.
*   **Internet Service and Add-ons:** Specific internet service types or the lack of services like Online Security and Tech Support can also influence churn likelihood.

# Recommendations

Strategic recommendations to reduce churn include:

1.  **Incentivize Longer Contracts:** Offer discounts or additional benefits for customers who switch from month-to-month to longer-term contracts.
2.  **Promote Automatic Payments:** Encourage customers to adopt automatic payment methods through incentives or easier setup processes.
3.  **Enhance Proactive Support:** Implement an early warning system for customers making multiple service calls and provide proactive outreach or support to address their issues before they churn.
4.  **Targeted Retention Campaigns:** Utilize the predictive model to identify high-risk customer segments (e.g., new customers, those with high monthly charges, electronic check users) and tailor retention offers or engagement programs.
5.  **Improve Service Quality:** Investigate the root causes behind high customer service call volumes and implement improvements to reduce issues and enhance customer satisfaction.

# Predictive Model

A predictive model was developed to forecast customer churn likelihood.

*   **Best Performing Model:** [Logistic Regression or Random Forest, based on your notebook output]
*   **Evaluation Metric (AUC-ROC):** [Insert the AUC score from your notebook output, e.g., 0.626]
*   **High-Risk Customers Identified:** [Insert the number of high-risk customers identified, e.g., 3]

The model's feature importance analysis highlighted **MonthlyCharges**, **TotalCharges**, **age**, **tenure**, and **CustomerServiceCalls** as the top predictors of churn.

*(Refer to `model_predictions.csv` for detailed test set prediction results and `feature_importance.csv` for the complete feature importance ranking.)*

# Visualizations

The notebook includes several visualizations to illustrate the data and findings:

*   Overall Churn Distribution
*   Churn Rate by Contract Type, Payment Method, and Internet Service
*   Distributions of Monthly Charges and Tenure by Churn Status
*   Relationship between Customer Service Calls and Churn Rate
*   Feature Importance Bar Chart
*   Model Comparison ROC Curve

*(Consider adding screenshots of your most impactful visualizations here to make your README more engaging visually.)*

# Conclusion

This project demonstrates an end-to-end approach to customer churn analysis, from data simulation and exploratory analysis to predictive modeling and actionable business recommendations. The developed model and the derived business insights offer valuable tools for implementing targeted retention strategies that can lead to significant revenue protection. This project demonstrates proficiency in data analysis, machine learning, and translating technical findings into actionable business recommendations.

# Author

Anirban roy
