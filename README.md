# Dynamic Pricing Strategy Project 📈🚗

Welcome to the Dynamic Pricing Strategy Project! This project aims to enhance pricing strategies for a ride-sharing service by analyzing various factors and implementing a dynamic pricing model.

## Project Overview 🎯

The goal of this project is to develop and evaluate a dynamic pricing model based on ride demand, supply, and historical costs. We aim to improve profitability by adjusting ride prices dynamically.

## Dataset Description 

The dataset used in this project includes information about ride requests and historical ride costs. The key columns in the dataset are:

- **Number_of_Riders**: Number of riders requesting a ride.
- **Number_of_Drivers**: Number of drivers available.
- **Location_Category**: Location of the ride (Urban, Suburban, Rural).
- **Customer_Loyalty_Status**: Loyalty status of the customer (Silver, Regular).
- **Number_of_Past_Rides**: Number of rides the customer has taken in the past.
- **Average_Ratings**: Average rating of the customer.
- **Time_of_Booking**: Time of day the ride is booked (Morning, Afternoon, Evening, Night).
- **Vehicle_Type**: Type of vehicle requested (Premium, Economy).
- **Expected_Ride_Duration**: Expected duration of the ride in minutes
- **Historical_Cost_of_Ride**: Historical cost of the ride.

## Approach 🛠️

### Data Loading and Exploration 📥

We start by loading the dataset and performing initial exploration to understand its structure and statistics. We use various data visualizations and statistical measures to gain insights.

### Data Visualization 📉

- **Scatter Plot**: Shows the relationship between `Expected_Ride_Duration` and `Historical_Cost_of_Ride`.
- **Box Plot**: Displays the distribution of `Historical_Cost_of_Ride` by `Vehicle_Type`.
- **Correlation Matrix**: Visualizes the correlation between numeric features.

### Dynamic Pricing Calculation 💡

We calculate dynamic pricing adjustments based on demand and supply multipliers:

- **Demand Multiplier**: Adjusted based on high and low demand percentiles.
- **Supply Multiplier**: Adjusted based on high and low supply percentiles.
- **Adjusted Ride Cost**: Calculated using demand and supply multipliers .

### Profitability Analysis 📈

We compute the profit percentage for each ride and categorize rides into profitable or loss-making. Visualizations include:

- **Donut Chart**: Displays the distribution of profitable and loss rides.
- **Scatter Plot**: Compares `Expected_Ride_Duration` with `adjusted_ride_cost`.

### Model Training and Prediction 🤖

A Random Forest Regressor model is trained to predict the adjusted ride cost based on features such as `Number_of_Riders`, `Number_of_Drivers`, `Vehicle_Type`, and `Expected_Ride_Duration`.

### Predictive Analysis 🔮

The model is used to make predictions for new data, and results are visualized to assess model performance.

## Files and Code Structure 📁

- `dynamic_pricing.csv`: The dataset used for analysis.
- `data_preprocessing_pipeline.py`: Code for preprocessing and handling missing values and outliers.
- `dynamic_pricing_model.py`: Code for calculating dynamic pricing, training the model, and making predictions.

## Installation and Requirements 🛠️

Ensure you have the following packages installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `plotly`
- `scipy`

You can install them using pip:

```bash
pip install pandas numpy scikit-learn plotly scipy
```

## Usage 🚀

1. **Load Data**: Load the dataset into a DataFrame.
2. **Preprocess Data**: Run the data preprocessing pipeline to clean and prepare the data.
3. **Calculate Dynamic Pricing**: Compute demand and supply multipliers and adjust ride costs.
4. **Train Model**: Fit the Random Forest model on the training data.
5. **Predict and Analyze**: Use the model to predict ride costs and analyze profitability.

## Conclusion 🎉

The Dynamic Pricing Strategy Project aims to refine pricing strategies and enhance profitability for ride-sharing services. By leveraging dynamic pricing based on demand and supply factors, we strive to optimize ride costs and improve overall performance.

For further details or questions, feel free to reach out!

---

Neharsha Vishnu Kanneganti
