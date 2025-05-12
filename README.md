# Coupon Acceptance Analysis
This project explores factors that influence whether drivers accept or reject driving coupons. Using a dataset from the UCI Machine Learning Repository, we analyze user demographics, driving context, and coupon characteristics to uncover behavioral trends and patterns in coupon redemption.
To identify and visualize the key differences between individuals who accept a driving coupon versus those who do not, using statistical analysis and Python-based data visualization.

## Exploratory Data Analysis
### Understand the Data and Data Collection
This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk.

- **Size:** 12,684 observations with 26 features

- **Label:**
  - Y = 1: Accepted the coupon (immediately or before expiration)
  - Y = 0: Rejected the coupon

- **Features:**
  - User attributes: Gender, age group, marital status, occupation, income, education, number of children, and behavior (e.g., frequency of visiting bars, restaurants, etc.)

  - Contextual attributes: Destination, passenger, weather, temperature, and time of day

  - Coupon attributes: Type of venue and time before expiration

### Data Cleaning
The dataset was examined for missing or problematic values, and the following potential data quality issues were identified.
- **Missing Data:**
The Car column contains 12,576 missing values out of 12,684 total rows—approximately 99.1% missing. This means only 108 rows have valid entries, making the column extremely sparse. Such limited information is unlikely to add value to the analysis and may introduce noise. Therefore, this column can be safely dropped.

Other columns with missing values include:

  - Bar: 107 missing

  - CoffeeHouse: 217 missing

   - CarryAway: 151 missing

   - RestaurantLessThan20: 130 missing

   - Restaurant20To50: 189 missing

Each of these represents less than 2% missing data, which is typically acceptable. In cases where missing values cannot be reliably imputed and account for less than 5% of the data, it is generally safe to ignore them in the analysis.

- **Duplicate Data:**
  There are 74 duplicate rows in the dataset, which have been removed.
### Data Visualization

