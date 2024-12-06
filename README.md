# Insurance Data Analysis Project
Overview
This project involves the analysis and feature exploration of an insurance dataset. The goal is to identify insights into key features such as vehicle_value, overnight_location, and voluntary_xs, as well as their relationship with the target variable, avg_claim_size. The project also addresses data quality issues, feature engineering, and skewed data treatment to improve predictive modeling.

## Key Objectives
Data Preprocessing:

### Handled missing data.
Performed data transformations for feature engineering.
Addressed skewed distributions in key numerical variables.
Feature Exploration:

### Identified important features such as vehicle_value, overnight_location, and voluntary_xs.
Explored relationships between features and avg_claim_size using visualizations.
Insights Generation:

### Observed trends in claim sizes based on vehicle value and age.
Noted the need to recalibrate premiums based on average claim size trends.
Modeling Preparation:

### Treated skewed data using transformations.
Selected the top features for modeling using feature importance techniques (e.g., Random Forest).
### Dataset Description
The dataset includes the following columns:

vehicle_value: Value of the insured vehicle.
overnight_location: Location where the vehicle is parked overnight.
voluntary_xs: Voluntary excess chosen by the policyholder.
avg_claim_size: Average size of claims for each policy.
Additional features: Vehicle age, make, policy duration, driver experience, claim severity, etc.
Methods Used
### Data Transformation:

Binning: Grouped vehicle_value and vehicle_age into bins (e.g., Low, Medium, High, Luxury).
Label Encoding: Encoded categorical variables for machine learning compatibility.
Feature Engineering:

### Engineered new features such as claim severity and average claim size.
Explored feature importance using Random Forest.
Data Visualization:

Bar plots and violin plots to analyze feature relationships.
Example:
Bar plot of vehicle_value_bin vs. avg_claim_size.
Violin plot for feature distributions.
Skewness Handling:

### Applied log transformations and binning to normalize skewed data.
Key Insights
Vehicle Value and Claims: Luxury vehicles tend to have lower average claim sizes compared to high-value vehicles.
Vehicle Age: Older vehicles (11–20 years) show lower claim sizes, but variability increases for very old vehicles (21+ years).
Overnight Location: Affects claim sizes significantly; further calibration may be required.
Voluntary Excess: Higher excess correlates with lower claim sizes, suggesting a behavioral trend in risk aversion.
### Setup Instructions
Prerequisites
Python 3.8+
Required Python Libraries:
pandas, numpy, seaborn, matplotlib
scikit-learn, ydata-profiling
statsmodels
### Installation
Clone this repository:

bash
Copy code
git clone https://github.com/username/insurance-analysis.git
cd insurance-analysis
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the analysis script:

bash
Copy code
python analysis.py
Usage
Run data_preprocessing.py for data cleaning and transformation.
Use feature_exploration.py to generate graphs and insights.
Apply modeling_preparation.py for creating datasets ready for machine learning.
### Visualization Examples
Bar Plot: Vehicle Value Bin vs. Average Claim Size

Violin Plot: Vehicle Value Bin vs. Average Claim Size

## Future Work
Develop a predictive model for avg_claim_size using selected features.
Implement automated anomaly detection for new incoming data.
Explore additional interactions between features (e.g., driver experience and claim severity).
Contributing
Contributions are welcome! Please submit a pull request or report issues.







