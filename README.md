# Datascience_Project


 ## [Real Estate Data ScrapingCleaning, and Analysis]

 
### 1-Objectives
The main goal of this project is to collect, clean, and analyze real estate property listings from leading property websites in Oman. The processed dataset can later be used for data analysis or building predictive models (such as predicting rental prices).

### 2-Websites Used
#### *Data Collection Sources:
opensooq.com
bayut.om

#### *Reference & Coding Help:
geeksforgeeks
chatgpt
khoula repositori --> Content folder
youtube

### 3-Steps Taken:

#### 1. Data Collection (Web Scraping)
Wrote custom Python scripts using requests and BeautifulSoup to scrape property listing data from both websites.

Handled pagination to collect data from all available listing pages.

Saved the raw data into structured CSV files for each website.

#### 2. Data Cleaning
Combined the data from both sources into a single DataFrame.

Cleaned column names and ensured consistent data types across columns.

Removed duplicates and handled missing values (e.g., filled missing sizes with the median value, locations from titles, etc.).

Split combined fields (such as "80 m2") into separate numeric and unit columns.

Standardized currency values.

#### 3. Feature Engineering
Created new features:

Price_per_SqM: Price divided by size (when available).

.Feature scaling: Applied normalization (e.g., MinMaxScaler) and Box-Cox transformations to numeric features.

.Categorical Encoding: Used one-hot encoding for variables like Listing_Type.

.Ensured all features were ready for further analysis or modeling.

### 4. Modeling Approach (if applicable)
.(Optional) Built simple regression models to predict price or price per square meter based on available features.

.Evaluated model performance using standard metrics.

### Usage
Run the Jupyter notebook(s) to reproduce the scraping, cleaning, and feature engineering steps.

The final cleaned dataset can be found in properties_cleaned.csv.

sklearn.ensemble 
