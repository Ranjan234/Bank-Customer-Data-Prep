# Bank-Customer-Data-Prep
Clean and explore bank customer data to prepare it for machine learning models

- Account information for 10,000 customers at a European bank, including details on their credit score, balance, products, and whether they have churned.

# The SITUATION 
 You've just  been as a Data scientist for the Bank of Maveland, the national bank in the country where data analysis is the most popular pastime

 # The ASSIGNMENT
 - The production team at the bank has noticed an uptick in customer churn and a decline in growth, and they want to find ways to reduce churn and appeal to new customers
 - You've been asked to prepare and explore a set of customer data that will be used for two machine learning projects: churn prediction & customer segmentation.

# The OBJECTIVES
 1. Join & QA the data
    * Import the data from both tabs in the "Bank_Churn_Messy" Excel file.
    * Use a left join to join "Account_Info" to "Customer_Info" using the CustomerID column.
    * Check for and remove duplicate rows and columns.
      
 2. Clean the data
    * Check the data types for each column and make any necessary fixes.
    * Replace missing values in categorical columns with "MISSING", and missing values in numeric columns with the median.
    * Profile the numeric columns in the data. Are there any extreme or non-sensical values? If so, impute them with the median of the column.
    * Combine any variations in country names in the "Geography" column to a single value per country.
   
 3. Explore feature relationships with customer churn
    * Build a bar chart displaying the count of churners (Exited=1) vs. non-churners (Exited=0).
    * Explore the categorical variables vs. the target, and look at the percentage of Churners by “Geography” and “Gender”
      Build box plots for each numeric field, broken out by churners vs. non-churners.
    * Build histograms for each numeric field, broken out by churners vs. non-churners.
      
 4. Prepare the data for modeling 
    * Create a new dataset that excludes any columns that aren’t be suitable for modeling.
    * Create dummy variables for categorical fields.
    * Create a new “balance_v_income” feature, which divides a customer’s bank balance by their estimated salary, then visualize that feature vs. churn status
   
   
