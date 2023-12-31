# Optimizing Instant Noodles Inventory in the Supply Chain with Machine Learning: A Regression Analysis

## Problem Description
   A Fast Moving Consumer Goods (FMCG) company entered into the instant noodles business two years back. Their higher management has noticed that there is a mismatch in the demand and supply. Where the demand is 
   high, supply is pretty low and vice-versa which results in a loss in inventory cost and ultimately loss to the company. Hence, the higher management wants to optimize the supply quantity in each and every 
   warehouse in the entire country.
   The objective of this exercise is to build a model, using historical data that will determine an optimum weight of the product to be shipped each time from the respective warehouse.

   ### Data Dictionary
   - Ware_house_ID: Unique identifiers for individual warehouses.
   - WH_Manager_ID: Unique identifiers for warehouse managers.
   - Location_type: Indicates the type of location where each warehouse is situated.
   - WH_capacity_size: Represents the capacity or size of each warehouse.
   - zone: Categorizes warehouses into specific zones.
   - WH_regional_zone: Assigns each warehouse to a regional zone.
   - num_refill_req_l3m: Records the number of refill requests received in the last 3 months.
   - transport_issue_l1y: Indicates if there have been any transport-related issues within the last year.
   - Competitor_in_mkt: Specifies the presence of competitors in the market.
   - retail_shop_num: Provides the number of retail shops associated with each warehouse.
   - wh_owner_type: Describes the ownership type of each warehouse.
   - distributor_num: Represents the number of distributors associated with each warehouse.
   - flood_impacted: Indicates whether a warehouse has been impacted by floods.
   - flood_proof: Specifies whether a warehouse is flood-proof.
   - electric_supply: Indicates the status of electric supply to each warehouse.
   - dist_from_hub: Represents the distance of each warehouse from the hub.
   - workers_num: Provides the number of workers employed at each warehouse.
   - wh_est_year: Represents the year in which each warehouse was established.
   - storage_issue_reported_l3m: Indicates whether any storage issues have been reported in the last 3 months.
   - temp_reg_mach: Specifies the presence of temperature regulation machinery at each warehouse.
   - approved_wh_govt_certificate: Indicates if each warehouse has an approved government certificate.
   - wh_breakdown_l3m: Indicates whether any breakdowns have occurred at each warehouse in the last 3 months.
   - govt_check_l3m: Indicates if government checks have been conducted for each warehouse in the last 3 months.
   - product_wg_ton: Represents the weight of the product in tons.

   ### Constructing a Regression Model - Steps
   
   1. Data Preparation and Analysis:

          - Explore and clean training data.
          - Analyze variable distributions and correlations.
          -  Encode categorical variables.
          -  Split data into independent and predictor variables.

   2.  Test Data Preprocessing:

           - Prepare test data using the same preprocessing steps
           
   3.  Regression Modeling:

           - Train a Linear Regression Model.
           - Evaluate Ensemble Learning Algorithms: Gradient Boost, AdaBoost, Random Forest, Bagging.
           
   4.  Hyperparameter Tuning:

           - Optimize model hyperparameters using Randomized Search Cross-Validation.
           
   5.   Model Predictions:

           - Use the best model to predict test data
           - Regression plot to visualize predicted vs. actual values.
           
   6.   Conclusion

### Findings:
After thoroughly assessing a range of regression algorithms, the Gradient Boosting method has emerged as the most precise option forthe regression task.
Through an extensive hyperparameter tuning process using Randomized Search Cross-Validation, our chosen GradientBoostingRegressor model has been optimized for peak performance with 'n_estimators' set to 100, 'max_depth' at 5, and a 'learning_rate' of 0.1.

Evaluation Metrics for the Best Model:

Mean Squared Error (MSE): 802,552.71
Root Mean Squared Error (RMSE): 895.85
R-squared (R^2): 0.99
