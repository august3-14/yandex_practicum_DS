# Statistical Data Analysis
You are an analyst for the popular scooter rental service GoFast. You have been provided with data on some users from multiple cities, as well as their trips. Your task is to analyze the data and test several hypotheses that could help the business grow.

To travel around the city, GoFast users rely on the mobile app. The service can be used in two ways:

Without a subscription:
* No subscription fee
* Cost per minute of a ride: 8 rubles
* Start fee (trip initiation): 50 rubles

With an Ultra subscription:
*Subscription fee: 199 rubles per month
* Cost per minute of a ride: 6 rubles
* No start fee

# Data Description
The main dataset contains information about users, their trips, and subscriptions.
Users — `users_go.csv`
| Column Name         | Description                                      |  
|---------------------|--------------------------------------------------|  
| **user_id**        | Unique user identifier                           |  
| **name**           | User's name                                      |  
| **age**            | User's age                                       |  
| **city**           | City of residence                                |  
| **subscription_type** | Subscription type (`free`, `ultra`)            | 

Rides - `rides_go.csv`
| Column Name  | Description  |  
|-------------|-------------------------------------------------------------|  
| **user_id**  | Unique user identifier                                     |  
| **distance** | Distance traveled by the user in the current session (meters) |  
| **duration** | Session duration (minutes) — time from "Start Trip" to "End Trip" |  
| **date**     | Date of the trip    

Subscriptions — `subscriptions_go.csv`
| Column Name          | Description                                       |  
|----------------------|---------------------------------------------------|  
| **subscription_type**  | Subscription type                               |  
| **minute_price**      | Price per minute for this subscription (rubles)  |  
| **start_ride_price**  | Price to start a ride (rubles)                   |  
| **subscription_fee**  | Monthly subscription fee (rubles)                |

During the study, we will analyze the data and test several hypotheses:
* `Hypothesis #1`: Users with a subscription spend more time on rides.
* `Hypothesis #2`: The average distance traveled by a subscribed user does not exceed the optimal trip distance.
* `Hypothesis #3`: Monthly revenue from subscribed users is higher than from regular users.

# Plan  
1. **Familiarization with the Data**  
2. **Data Preprocessing**  
3. **Exploratory Data Analysis**  
   - 3.1. **City**  
   - 3.2. **Subscription Type**  
   - 3.3. **Age**  
   - 3.4. **Distance**  
   - 3.5. **Duration**  
4. **Merging Data and Comparing Metrics**  
   - 4.1. **Creating Datasets for Statistical Analysis**  
   - 4.2. **Comparing Data Distributions**  
5. **Revenue Calculation**  
6. **Hypothesis Testing**  
   - 6.1. **Hypothesis 1: Ride Duration**  
   - 6.2. **Hypothesis 2: Distance**  
   - 6.3. **Hypothesis 3: Revenue**  
   - 6.4. **Customer Support Requests**  
7. **Marketing Activities Calculation**  
   - 7.1. **Subscription Promo Codes**  
   - 7.2. **Push Notification Campaigns**  
8. **Conclusions**  
