# **Project Overview**

- Objective: Enhance business performance by identifying factors influencing hotel booking cancellations.
- Dataset: 119,390 rows and 29 columns.
- Data Cleaning: Replaced missing values with:
  0 for columns children, agent, and company.
  unknown for the city column.
- Analysis Goal: Obtain insights into customer behavior and factors affecting hotel booking cancellations.

# **Problem Background**
The company aims to improve its business performance. The data analysis team has been tasked with uncovering insights into customer behavior in booking hotel tickets and identifying factors influencing hotel booking cancellations.

# **Data Preprocessing**
- Replaced undefined with No Meal in the meal column, assuming the customer did not book a meal package.
- Replaced undefined with TA/TO in the distribution channel column, as TA/TO is the majority value.
- Data Type Adjustment: Converted the children, agent, and company columns from float to integer.
- Feature Engineering:
Created a new column total_guest by summing adults, children, and baby, and removed rows with 0 values.
Created a new column stay_duration by summing stays_in_weekend_nights and stays_in_weekdays_nights, and removed rows with 0 values.

# **Univariate Analysis**
Most features in the dataset have a right-skewed distribution, indicating that most values are lower with some extreme high values. These extremes may result from data entry errors, such as having 9 or 10 babies in one booking, which is highly unlikely.

# **Monthly Hotel Booking Analysis Based on Hotel Type**
This analysis focuses on booking trends over time for different hotel types. The highest bookings for both types of hotels occur in June and July, coinciding with school holidays and festive seasons. In August and September, there is a significant drop in bookings. For other months, there are no long holidays or weekends, resulting in lower booking volumes. In December, bookings rise again due to school holidays, Christmas, and New Year.

# **Impact Analysis of Stay Duration on Hotel Booking Cancellation Rates**
This analysis examines the relationship between stay duration and cancellation rates. The longer the stay duration, the higher the likelihood of cancellations. For city hotels, the cancellation probability is much higher than for resort hotels.

# **Impact Analysis of Lead Time on Hotel Booking Cancellation Rate**
This analysis explores the relationship between lead time (time between booking and check-in) and cancellation rates. The fact is the longer the lead time, the higher the likelihood of cancellations.

# **Recommendations**
- Offer flexible booking and cancellation policies, especially for long-duration stays, to manage and reduce cancellations.
- Target promotions and discounts during off-peak months to balance the booking volumes throughout the year.
- Use customer behavior data to create personalized offers and packages, especially for city hotel customers, to enhance booking retention.
- Create a loyalty program to reward loyal customers and provide incentives for them not to cancel their bookings. For example, offer loyalty points that can be redeemed for discounts or additional services.
- 
