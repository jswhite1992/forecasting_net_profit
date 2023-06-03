# forecasting_net_profit

This project uses the Prophet library to perform time series forecasting on MercadoLibre's stock prices and Google search traffic.

## Dependencies

This project uses the following libraries:

- Python 3.x
- Pandas
- hvplot
- Facebook Prophet
- Google Colab
- Holoviews

## Steps

The process for this project involves:

1. Read in MercadoLibre's historical stock data and Google search traffic data.
2. Clean and preprocess the data for use in the Prophet model. This involves:
   - Resetting the DataFrame index
   - Renaming the columns to the required 'ds' (datestamp) and 'y' (value to predict)
   - Dropping any NaN values
3. Create a Prophet model and fit it to the data.
4. Make future predictions using the Prophet model's `predict` method.
5. Visualize the forecasted data using Prophet's `plot` function and `plot_components` function to see trend and seasonality.
6. For the Google search traffic data, we further analyzed the time of day and day of the week that exhibited the most search traffic.
7. For the sales forecast, we additionally provided the sum of the forecasted values for a quarter (90 days) into the future, providing expected total sales, best case, and worst-case scenarios.

## Results

The Prophet model provided forecasts for the stock prices and Google search trends. The model was also used to predict the next quarter's sales figures, assisting the finance team with their budgeting and planning.

## Caveats

These predictions are only estimates based on historical data, and actual future values may vary due to unforeseen circumstances.

## Acknowledgements

This project utilizes data from MercadoLibre and Google trends.
