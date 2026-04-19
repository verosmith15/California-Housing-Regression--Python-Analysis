# California Housing Price Prediction 

## Project Overview
In this project, I developed a Machine Learning model to predict median house values in California. As an economist, I focused on analyzing how household income and geographical location (ocean proximity) influence real estate market prices.

## Tech Stack
* **Language:** Python 
* **Environment:** Google Colab
* **Libraries:** Pandas (Data Manipulation), Matplotlib (Visualization), Scikit-Learn (Machine Learning), Numpy (Calculations)

## Key Steps & Methodology

### 1. Data Cleaning (ETL)
* Identified and handled missing values in the `total_bedrooms` feature using a median imputation strategy.
* Performed **One-Hot Encoding** on categorical variables (Ocean Proximity) to prepare the data for the regression model.

### 2. Exploratory Data Analysis (EDA)
* Identified a price cap at **$500,001** in the dataset, which is a critical observation for model accuracy.
* Confirmed a strong positive correlation between **Median Income** and **House Value**.

### 3. Feature Engineering
* Developed new economic ratios to improve model performance:
    * `rooms_per_household`
    * `bedrooms_per_room`
    * `population_per_household`

### 4. Machine Learning Modeling
* Implemented a **Linear Regression** model using a 80/20 train-test split.
* **Evaluation Metric:** Achieved a Root Mean Squared Error (RMSE) of approximately **$72,668**.

## Results & Visualizations
*(Aquí insertas las imágenes que guardaste de Colab)*

## Future Improvements
* Test non-linear models like **Random Forest** or **XGBoost** to reduce the RMSE.
* Perform outlier removal for the capped price values ($500k).
