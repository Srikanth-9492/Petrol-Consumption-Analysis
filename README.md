**Project Title: Petrol Consumption Analysis**

### **Objective**
The primary goal of this project is to build a linear regression model to predict petrol consumption based on several key features. The analysis involves exploring the dataset, preprocessing the data, training a model, and evaluating its performance.

### **Dataset**
* **Source:** `oil_consumption.csv`
* This project uses a dataset with 48 entries and the following columns:
    * **Independent Variables (Features):**
        * `Petrol_tax`
        * `Average_income`
        * `Paved_Highways`
        * `Population_Driver_licence(%)`
    * **Dependent Variable (Target):**
        * `Petrol_Consumption`

### **Methodology & Workflow**
1.  **Data Exploration & Visualization (EDA):**
    * The dataset was loaded and inspected for shape, data types, and missing values (none were found).
    * Descriptive statistics were calculated to get a summary of the data.
    * **Histograms** were plotted to visualize the distribution of each feature.
    * **Scatter plots** and a **correlation heatmap** were created to analyze the relationships between the features and the target variable (`Petrol_Consumption`).

2.  **Data Preparation:**
    * The dataset was split into features (X) and the target variable (y).
    * Features were scaled using **StandardScaler** to normalize their range and ensure they are on a common scale.
    * The data was split into training (80%) and testing (20%) sets.

3.  **Model Building:**
    * A **Linear Regression** model was chosen for this regression task.
    * The model was trained on the scaled training data.

4.  **Model Evaluation:**
    * The model's performance was tested on the unseen test data.
    * A scatter plot of **Actual vs. Predicted** values was generated to visually assess performance.

### **Results & Insights**
* The model yielded the following evaluation metrics on the test set:
    * **R-squared (R2):** 0.39
    * **Mean Squared Error (MSE):** 4083.26
    * **Root Mean Squared Error (RMSE):** 63.90
* **Key Finding:** The proportion of the population with a driver's license showed the strongest positive correlation with petrol consumption.
* **Insight:** Petrol tax showed a negative correlation, suggesting it can be a tool to influence fuel usage.

### **Technologies Used**
* **Python**
* **Pandas:** For data manipulation and analysis.
* **Scikit-learn:** For data preprocessing and building the regression model.
* **Matplotlib & Seaborn:** For data visualization.
* **Google Colab:** As the development environment.
