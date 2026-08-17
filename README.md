## **Zomato Restaurants, Cuisine and Customer Preference Dashboard**

**Project Overview**

This Zomato project analyses the Restaurant data by working on around 19000 rows using SQL and PowerBI to generate insights about the Cuisines, Dishes, Restaurants and Customer performance across various Locations in Bangalore City.

This Dashboard uses various measures such as DAX calculations and interactive visualization to transform raw data so to generate meaningful insights which may help business gain the understanding of how Restaurants perform.

**DASHBOARD PREVIEW**
<img width="1603" height="899" alt="Dashboard Overview" src="https://github.com/user-attachments/assets/b22c09ed-dcc6-4d1c-ad22-32dc326f8402" />


**Tools Used**
- Microsoft PowerBI
- DAX Calculation
- Data Visualization
- Data Modeling
- Power Query

## **DATASET**

https://github.com/Bhawesh-J/Zomato-PowerBI-Dashboard/blob/main/Zomato_cleaned_data.csv

The dataset contains various columns including:
- Restaurant Name
- Table Booking
- Rating
- Votes
- Location
- Dishes Liked
- Cuisines
- Cost


## **Dashboard Pages**

**1. Overview**

**Purpose:**
Provides the summary of the Overall Report.

**Includes**

- Restaurants By Location
- Top Rated Restaurants
- Table Booking vs online order Cost Analysis
- Ratings and Cost Analysis of Costliest Restaurants
- Price and Vote Relationship in Priciest Locations

<img width="1603" height="899" alt="Dashboard Overview" src="https://github.com/user-attachments/assets/5681741a-c01b-48e8-84d9-0c3cdf1a3096" />

**2. Cuisine Insights**

**Purpose:**
To get insights on Cuisine and Dishes and their Relationship.

**Includes**

- Most Offered Cuisines
- Most liked Dishes
- Restaurants Offering the most Liked Dishes in the Town
- Location Wise Average Food Cost
- Votes and Ratings Relationship

<img width="1602" height="900" alt="Cuisine Insight" src="https://github.com/user-attachments/assets/cf711450-2237-4c54-917a-396ba108793b" />

## **Data Modelling and Calculations**

Some of the DAX measures that I have Created:

**1. Total Cuisines**

Total cuisines offered = COUNT(cuisines_table[cuisines])

**2. Average Cost**

Average Cost = AVERAGE(fact_table[cost(2 People)] )

**3. Distinct Names**

Distinct Names = DISTINCTCOUNT(fact_table[name])

**4. Total Restaurant**

Total Restaurants = DISTINCTCOUNT(fact_table[name] )

**5. Restaurants with Online Order**

Rest. with online order = CALCULATE(DISTINCTCOUNT(fact_table[name]), (fact_table[book_table]) = "No")

## **Key Insights**

- North Indian Cuisine is the Most Offered Cuisine in Bangalore Indicating that it has a high Popularity in the region, but the top 5 dishes liked are not North Indian.
- A strong relationship cannot be established between Ratings and Votes.
- We can see that as the cost of the food increases, ratings generally tend to increase. Also after a certain threshold of food price which is 1500-1700, most ratings are in the range of 4+ which
  means that at this and above price range, the food quality and services are typically similar to restaurants offering food at higher prices.  
- Also most popular outlets are the one where price range is less than 2500 rupees. Also Votes significantly decrease as the price climbs higher than 3000 rupees.
- The priciest location tend to have high ratings while less votes meaning that the locations offer better food, but are less popular.
- The Restaurants offering table booking tend to be 2x more costly than one that are offering online orders which could mean that the restaurants might be very busy as charging 2x the price is something that many
  restaurants don't do. 

## **Skills Demonstrated**

- Data Cleaning
- Data Modeling
- Data Interpretation
- DAX Calculations
- Interactive Design
- Business Analysis
- Data Storytelling








