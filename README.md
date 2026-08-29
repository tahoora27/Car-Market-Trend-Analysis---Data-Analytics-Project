🚗 Car Market Trends Analysis using CarDekho Dataset
📌 Project Overview

This project analyzes the used-car market using the CarDekho dataset to identify the key factors that influence the resale value of used cars.

The analysis uses Exploratory Data Analysis (EDA) to examine relationships between car prices and vehicle characteristics such as car age, kilometers driven, current price, fuel type, seller type, transmission, previous ownership, and car brand.

A major focus of the project is to calculate the resale value percentage of each vehicle and identify the characteristics that help cars retain their market value.

🎯 Problem Statement

Analyzing the Factors Affecting the Resale Value of Used Cars and Identifying the Characteristics That Help Cars Retain Their Market Value.

🎯 Objectives

The main objectives of this project are:

To understand the structure and characteristics of the CarDekho used-car dataset.
To clean and prepare the dataset for analysis.
To identify patterns and trends in used-car prices.
To analyze the relationship between car age and resale value.
To investigate the impact of kilometers driven on resale value.
To analyze how fuel type, transmission, seller type, and previous ownership affect resale value.
To compare resale performance across different car brands.
To identify the characteristics associated with better value retention.
To derive meaningful business insights from the used-car market data.
📊 Dataset Description

The dataset contains 301 records and 9 attributes related to used cars.

Column	Description
Car_Name	Name/model of the car
Year	Manufacturing year of the car
Selling_Price	Selling price of the used car
Present_Price	Present/original market price of the car
Kms_Driven	Total kilometers driven
Fuel_Type	Fuel type of the vehicle
Seller_Type	Type of seller
Transmission	Transmission type
Owner	Number of previous owners
Dataset Characteristics
Original Records: 301
Original Features: 9
Missing Values: None
Duplicate Records: 2
Records after duplicate removal: 299
🔍 Feature Engineering

To make the analysis more relevant to the problem statement, additional features were created.

1. Car Age

Car age was calculated using the manufacturing year:

Car_Age = 2018 - Year

The reference year 2018 corresponds to the latest year available in the dataset.

2. Depreciation

The absolute difference between present price and selling price was calculated as:

Depreciation = Present_Price - Selling_Price
3. Resale Value Percentage

The percentage of the present price retained by the car was calculated as:

Resale_Value_Percentage = (Selling_Price / Present_Price) * 100

This metric is the primary measure used to analyze value retention.

4. Brand

The car name was processed to derive an approximate car brand for brand-level analysis.

🛠️ Technologies Used
Programming Language
Python
Development Environment
Google Colab / Jupyter Notebook
Libraries
Pandas – Data loading, cleaning, transformation, and analysis
NumPy – Numerical computations
Matplotlib – Data visualization
Seaborn – Statistical visualization
🔬 Exploratory Data Analysis

The project includes the following stages of EDA:

1. Data Understanding
Dataset shape
Data types
Statistical summary
Unique values
Missing-value analysis
2. Data Cleaning
Missing-value check
Duplicate detection
Duplicate removal
Data validation
3. Univariate Analysis

Analysis of individual variables such as:

Selling Price
Present Price
Car Age
Kilometers Driven
Fuel Type
Seller Type
Transmission
Previous Ownership
4. Bivariate Analysis

Relationships investigated include:

Car Age vs Selling Price
Car Age vs Resale Value
Kilometers Driven vs Selling Price
Kilometers Driven vs Resale Value
Present Price vs Selling Price
Fuel Type vs Resale Value
Transmission vs Resale Value
Seller Type vs Resale Value
Previous Owners vs Resale Value
5. Brand Analysis
Number of cars by brand
Average selling price by brand
Average resale value by brand
6. Correlation Analysis

A correlation matrix and heatmap were used to understand relationships between numerical variables.

7. Outlier Analysis

Boxplots were used to identify potential outliers in:

Selling Price
Present Price
Kilometers Driven
Resale Value

Outliers were investigated rather than automatically removed, as extreme values may represent genuine vehicles in the used-car market.

📈 Key Insights

The analysis focuses on determining how different factors influence used-car value retention.

Some important observations include:

Car age is an important factor associated with resale value, with older vehicles generally showing lower value retention.
Kilometers driven provides an indication of vehicle usage and can influence the selling price and resale value.
Present price has a strong relationship with selling price, as higher-value vehicles generally have higher selling prices.
Fuel type, transmission, and seller type show differences in resale-value patterns.
Previous ownership can influence resale value, although categories with fewer observations should be interpreted carefully.
Brand-level analysis can help identify vehicles that demonstrate stronger value retention.
The Resale Value Percentage provides a more meaningful measure of value retention than selling price alone.

Note: Insights are based on the observations in this dataset and should not be generalized to the entire used-car market without additional data.

👥 End Users

The analysis can be useful for:

Used-Car Buyers – To identify vehicles with better value retention.
Car Sellers/Owners – To understand factors affecting resale prices.
Car Dealers – To support pricing and inventory decisions.
Automotive Businesses – To understand used-car market trends.
Market Analysts – To analyze pricing and resale patterns.
📂 Project Structure
Car-Market-Trends-Analysis/
│
├── Car Market Trends Analysis with Car Dekho Data.csv
│
├── Car_Market_Trends_Analysis.ipynb
│
├── README.md


🚀 How to Run the Project
Option 1: Google Colab
Open the .ipynb notebook in Google Colab.
Upload the CarDekho CSV dataset when prompted.
Run the notebook cells sequentially.
Review the generated visualizations and insights.
Option 2: Local Jupyter Notebook

Clone the repository:

git clone https://github.com/your-username/Car-Market-Trends-Analysis.git

Navigate to the project directory:

cd Car-Market-Trends-Analysis

Install the required libraries:

pip install pandas numpy matplotlib seaborn

Open the notebook:

jupyter notebook

Run the cells sequentially.

📊 Results

The project produces several visualizations to understand used-car market behavior, including:

Selling price distribution
Car age distribution
Kilometers driven distribution
Fuel-type distribution
Car age vs resale value
Kilometers driven vs resale value
Present price vs selling price
Resale value by fuel type
Resale value by transmission
Resale value by seller type
Resale value by previous ownership
Brand-wise resale value
Correlation heatmap
Outlier analysis
💡 Conclusion

This project provides an exploratory analysis of the CarDekho used-car dataset with a focus on resale value and value retention.

The analysis demonstrates that factors such as vehicle age, kilometers driven, present price, fuel type, transmission, seller type, ownership history, and brand can be associated with differences in used-car selling prices and resale value.

The project provides data-driven insights that can help buyers, sellers, dealers, and automotive businesses better understand factors influencing the used-car market.

🔮 Future Scope

The project can be extended in the future by:

Using a larger and more recent used-car dataset.
Building a machine learning model to predict selling price.
Developing a car recommendation system based on resale value.
Comparing used-car trends across different cities or regions.
Incorporating additional factors such as insurance, service history, accident history, and vehicle condition.
Creating an interactive dashboard using Power BI, Tableau, or Streamlit.
👩‍💻 Author

Syeda Tahoora Fatima

Project Type

Exploratory Data Analysis | Data Analytics | Car Market Trend Analysis

⭐ Acknowledgement

This project was developed for educational and analytical purposes using the CarDekho dataset.
