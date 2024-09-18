# Uber-and-Lyft-model-prediction

This repository contains a project aimed at predicting ride prices for Uber and Lyft using regression analysis. The goal is to build a model that accurately estimates the cost of a ride based on various features such as distance, cab type, ride type, and other relevant factors.

# Table of Contents
- Project Overview
- Dataset Description
- Data Preprocessing
- Exploratory Data Analysis
- Modeling
- Evaluation
- Results and Conclusions
- Requirements
- Usage
- Project Structure
- License

  
# Project Overview
Ride-sharing services like Uber and Lyft have become integral to urban transportation. Understanding and predicting ride prices can benefit both consumers and service providers by enhancing pricing strategies and budgeting. This project develops a regression model to predict ride prices based on features such as distance, cab type, ride type, and other factors.

# Dataset Description
The dataset used in this project includes ride information from Uber and Lyft, comprising the following features:

- Distance: The distance of the ride.
- Cab Type: The service provider (Uber or Lyft).
- Ride Type (Name): Specific service levels (e.g., UberX, Lyft Lux).
- Source and Destination: Pickup and drop-off locations.
- Price: The cost of the ride (target variable).
Weather Conditions: Weather data at the time of the ride, including short_summary and icon.

# Data Preprocessing
Data preprocessing steps undertaken include:

- Handling Missing Values: Checked for and addressed any missing or null values to ensure data integrity.
- Outlier Removal: Removed outliers in the price column using the Interquartile Range (IQR) method to improve model performance.
- Encoding Categorical Variables: Applied one-hot encoding to convert categorical features (cab_type, name, source, destination) into numerical format suitable for regression analysis.
- Feature Selection: Selected relevant features based on correlation analysis, focusing on those that significantly impact the ride price.

# Exploratory Data Analysis
- Correlation Analysis: Assessed the relationship between features and the target variable to identify significant predictors.
- Visualizations: Created scatter plots and box plots to visualize data distributions and relationships.

# Hypothesis Testing: Formulated and tested hypotheses regarding factors affecting ride prices, such as the impact of distance and cab type.
Modeling
- Data Splitting: Divided the dataset into training and testing sets using a 70-30 split to evaluate model performance on unseen data.
- Pipeline Creation: Utilized scikit-learn's Pipeline and ColumnTransformer to streamline preprocessing and modeling steps.
- Regression Model: Trained a linear regression model to predict ride prices based on the selected features.

# Evaluation

Evaluated the model using the following metrics:

- R-squared (R²) Score: Measures the proportion of variance in the dependent variable predictable from the independent variables.
- Mean Squared Error (MSE): The average squared difference between actual and predicted prices.
- Root Mean Squared Error (RMSE): The square root of MSE, providing error in the same units as the target variable.
- Mean Absolute Error (MAE): The average absolute difference between actual and predicted prices.

# Visual Evaluation:

- Actual vs. Predicted Plot: Plotted actual and predicted prices to visually assess model performance.
- Scatter Plot with Best Fit Line: Plotted predicted values against actual values with a best fit line to evaluate the model's accuracy.

# Results and Conclusions
- High R² Score: The model achieved a strong R² score (e.g., ~0.80), indicating that it explains a significant portion of the variance in ride prices.
- Acceptable Error Margins: Error metrics like RMSE ($3.20) and MAE ($2.50) suggest that the model's predictions are reasonably accurate compared to the average ride price.
- Hypothesis Validation: The analysis supports the hypothesis that the regression model can predict ride prices with reasonable accuracy.

# Recommendations:
- Feature Enhancement: Incorporate additional features like time of day or traffic conditions to potentially improve the model.
- Advanced Modeling: Explore regularization techniques or advanced models like Random Forests to enhance predictive performance.

## Requirements
- Python 3.6 or higher

### Required libraries:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

### Usage

Clone the Repository:

bash
Copy code
git clone https://github.com/VincentDao25/Uber-and-Lyft-model-prediction.git
Navigate to the Directory:

bash
Copy code
cd Uber-and-Lyft-model-prediction
Install Dependencies:

Ensure you have a Python environment set up and install the required packages:

bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook:

Open the Jupyter Notebook to explore the analysis:

bash
Copy code
jupyter notebook "Uber and Lyft.ipynb"
Execute the Notebook:

Run each cell sequentially to reproduce the results.
Ensure the dataset is placed in the correct directory or adjust the file paths accordingly.
Project Structure
Uber and Lyft.ipynb: The main Jupyter Notebook containing the code, analysis, and visualizations.
requirements.txt: A list of required Python packages.
data/: Directory where the dataset is stored (ensure the dataset is placed here).
images/: Contains any images or plots generated during the analysis (if applicable).
README.md: This Readme file.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to contribute to this project by submitting issues or pull requests. Your feedback is valuable and helps improve the analysis and modeling approach.

Contact Information:

Author: Vincent Dao
