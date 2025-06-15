# Laptop-price-analysis

LAPTOP PRICE ANALYSIS USING MACHINE LEARNING FOR FINANCIAL INSIGHT

PROJECT OVERVIEW

This project focuses on analyzing and predicting laptop prices using a structured dataset that includes technical specifications such as processor, RAM, screen features, storage, and GPU. The objective is to build a machine learning model that estimates the price of a laptop based on its specifications, enabling better pricing strategy, value assessment, and product comparison from a finance analyst's perspective.

OBJECTIVES

Understand how different laptop specifications influence the final retail price
Clean and preprocess the dataset for machine learning
Visualize key variables and their relationship with price
Build and evaluate a regression model to predict laptop prices
Generate actionable insights for financial and market analysis

TOOLS AND TECHNOLOGIES USED

Python (Pandas, NumPy, Matplotlib, Seaborn)
Jupyter Notebook, VS Code
Machine Learning: Linear Regression
Optional: SQL and Excel for raw data review

DATA OVERVIEW

The dataset consists of 1275 laptops with 23 features each. Important fields include:
Company, Product, TypeName, Inches, Ram, OS, Weight, Price_euros, Screen details, Screen Resolution, Touchscreen, IPSpanel, RetinaDisplay, CPU specs, Storage (Primary and Secondary), GPU specs

DATA CLEANING AND PREPROCESSING

There were no missing values in the dataset.
All string-type features were standardized (e.g., lowercase, formatting).
Categorical variables were label encoded or one-hot encoded where necessary.
Target variable: Price_euros
Independent features included both numerical and transformed categorical data.
Unnecessary fields such as Product ID were dropped.
Units (GB, GHz) were stripped and converted to numeric formats for modeling.

FEATURE EXPLORATION

Company and TypeName provided insights into brand-based pricing differences
RAM and CPU frequency had clear linear relationships with price
Storage type (SSD, HDD, Hybrid) influenced pricing more than storage size alone
Features like Touchscreen, Retina Display, and IPSpanel also affected pricing positively
Scatter plots showed that higher CPU frequency generally paired with more RAM and a higher price
Screen size (inches) had a less direct impact compared to resolution and panel type

UNIVARIATE VISUAL ANALYSIS

Bar plots were used to analyze distributions for features like Company, OS, RAM, and Screen type
Pie charts showed the share of models with Touchscreen, IPSpanel, and GPU manufacturers
High variation was observed in RAM (2GB to 64GB), and storage configurations ranged widely
Most laptops were in the 14–15.6 inch screen size category
SSD was the most common primary storage type, followed by HDD and Flash Storage

BIVARIATE ANALYSIS

Price was plotted against categorical features using box and bar plots
Higher prices were associated with macOS and Windows compared to Linux or No OS
Laptops with Retina Display or Touchscreen had consistently higher prices
Bar plots showed dual storage configurations increased average pricing
Screen resolution and display type were positively correlated with pricing

MODELING

A Linear Regression model was used to predict laptop price
Data was split into training and testing sets (80/20)
Model trained using sklearn’s LinearRegression class
Evaluation metrics included Mean Squared Error and R² Score
Scatter plot showed predicted vs actual prices for model validation
The model provided a good baseline for further improvement using advanced models

RESULTS AND INSIGHTS

Laptop price is significantly influenced by brand, RAM, CPU frequency, GPU, and storage type
Retina displays and touch-enabled screens command a premium
Mid-tier brands (HP, Dell, Lenovo) offer a broad price range depending on features
Apple laptops had consistently higher prices for equivalent hardware
High RAM and fast CPUs are strong indicators of high pricing, but not always of value

CONCLUSION

This project demonstrated a full pipeline for data cleaning, exploration, and predictive modeling using real-world laptop data. By examining relationships between specifications and pricing, it offers a practical framework for understanding laptop market trends. The regression model sets a strong baseline, and additional refinements (e.g., Random Forest or XGBoost) can enhance prediction accuracy for more advanced financial applications.
