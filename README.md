# Context: Course assignment
This is my solution for coding assignment in Supervised Learning course.

**What was the main goal?**
The goal of this assignment was to implement simple linear regression on given dataset both with and without using scikit-learn package.
- Target variable: price
- Explanatory variable: square footage of the apartments interior living space

**What were the prescribed tasks and steps to accomplish it?**
1. Import the data “kc_house_sales.csv”
2. Implement simple linear regression with scikit
3. Implement simple linear regression without scikit package (Start with β_0=0, β_1=0, and α=?, Run for 1,000 iterations)
4. Print and plot mean squared error per epoch
5. Scatter plot the variables as well as the estimated regression line

# Data: House prices
The dataset consists of house prices from King County an area in the US State of Washington, this data also covers Seattle. The dataset was obtained from Kaggle. This data was published/released under CC0: Public Domain.

| Column | Descritption |
| --- | --- |
| id | Unique ID for each home sold |
| date | Date of the home sale |
| **price** | **Price of each home sold** |
| bedrooms | Number of bedrooms |
| bathrooms | Number of bathrooms, where .5 accounts for a room with a toilet but no shower |
| **sqft_living** | **Square footage of the apartments interior living space** |
| sqft_lot | Square footage of the land space |
| floors | Number of floors |
| waterfront | A dummy variable for whether the apartment was overlooking the waterfront or not |
| view | An index from 0 to 4 of how good the view of the property was |
| condition | An index from 1 to 5 on the condition of the apartment |
| grade | An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high quality level of construction and design |
| sqft_above | The square footage of the interior housing space that is above ground level |
| sqft_basement | The square footage of the interior housing space that is below ground level |
| yr_built | The year the house was initially built |
| yr_renovated | The year of the house's last renovation |
| zipcode | What zipcode area the house is in |
| lat | Lattitude |
| long | Longitude |
| sqft_living15 | The square footage of interior housing living space for the nearest 15 neighbors |
| sqft_lot15 | The square footage of the land lots of the nearest 15 neighbors  |

# Process and results
Comments on process are directly in the code. Here is quick overview:
1. Data load and simple Exploratory Data Analysis (EDA). For this purpose, several "warm up" question were asked.
2. Implement linear regression using scikit-learn library: transform and split data, create and fit model, extract the linear regression equation.
3. Implement linear regression **without** using scikit-learn library: transform and split data, write and apply function for gradient descent, write and apply function for prediction, extract the linear regression equation.
4. Calculate evaluation metrics for both and compare, plotting both linear regression equations.

Few very distant outliers were identified in during EDA. Thus, for both point 2. and 3. two versions of data were used: A) **With** outliers (OL), B) **Without** outliers (WOL) to see inspect their influence.

# Disclaimer
Visualization map with plotly wasn't done by me. It was given by lecturer to show us location of the houses.
