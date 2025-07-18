# Monthly-Electricity-Production
- $\textbf{Author}$: Patrick Mthisi
- $\textbf{Contact details}$: patrickmthisi@hotmail.com

## Project objectives and description:
This notebook demonstrates an end-to-end time series forecasting project for electricity production, including model fitting, sliding window cross-validation, and construction of a time series ensemble model based on the top five best-performing models, which include but are not limited to AutoARIMA, Prophet, TBATS, reduced regression methods using random forest, LightGBM, etc.

The following important time series forecasting concepts are explored in this end-to-end project:
1. A suite of classical and ML-based time series models was implemented, and the 5 best-performing pipelines were selected using sliding window cross-validation and several evaluation metrics such as MAPE, RMSE, etc.
2. Bayesian hyperparameter optimization was implemented to select the optimal hyperparameters for each of the 5 selected pipelines.
3. A blended model consisting of the tuned best-performing pipelines from step (2) was developed, and an in-sample fit was displayed.
4. Rolling Forecast:
    - After training the final model, we provide a 12-month forecast of monthly electricity production.
5. Model Evaluation:
    - The forecasted values from step (4) were compared against the actual values from the out-of-sample set.
    - The final predictions and actual validation data are plotted for visualization.
6. Next Steps: We also mention possible improvements, such as experimenting with power transformations (e.g., BoxCox, log, sqrt, etc) for further performance optimization.


$\textbf{Bonus}$: EDA was performed, including ADF and KPSS stationarity tests, as well as STL-based time series decomposition.

## Conclusion and further work...
In this comprehensive project, we achieved impressive results, with in-sample RMSE  and MAPE  values of 2.84 and 2.03%, respectively. Our out-of-sample RMSE and MAPE were 4.77 and 3.07%, respectively. These metrics are comparable to the majority of work presented on Kaggle for this dataset.

![Out-of-sample forecast](electricity_prod_forecast_oos.png)

For reference, please see https://www.kaggle.com/datasets/shenba/time-series-datasets/code. We did not experiment with power transforms such as Box-Cox; perhaps that is an extension of the work that can be implemented.


