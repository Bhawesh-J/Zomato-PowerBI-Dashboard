## **Zomato Restaurants, Cuisine and Customer Preference Dashboard**

**Project Overview**

This Zomato project analyses the Restaurant data using PowerBI to generate insights about the Cuisines, Dishes, Restaurants and Customer performance across various Locations in Bangalore City.

This Dashboard uses various measures such as DAX calculations and interactive visualization to transform raw data so to generate meaningful insights which may help business gain the understanding of how Restaurants perform.

**DASHBOARD PREVIEW**
<img width="1920" height="1080" alt="Overview" src="https://github.com/user-attachments/assets/6d42aac6-ec7d-420f-b939-b6f66aa1e57a" />

**Tools Used**
- Microsoft PowerBI
- DAX Calculation
- Data Visualization
- Data Modeling
- Power Query

## **DATASET**

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

<img width="1920" height="1080" alt="Overview" src="https://github.com/user-attachments/assets/d19ecf16-4709-46a3-b977-8c469d70820f" />


**2. Location Analysis**

**Purpose:**
Analyses Restaurants Performance In the Bangalore Location.

**Includes**

- Restaurants Offering Online Services
- Average Rating vs Minimum Rating in a Location
- Location Wise Average Food Cost
- Restaurants with Maximum Cuisine Diversity and their Popularity

<img width="1920" height="1080" alt="Location Analysis" src="https://github.com/user-attachments/assets/3f5d357f-2bf1-4639-aef8-f402e6c590d4" />

**3. Cuisine Insights**

**Purpose:**
To get insights on Cuisine and Dishes and their Relationship.

**Includes**

- Most Offered Cuisines
- Most liked Dishes
- Restaurants Offering the most Liked Dishes in the Town

<img width="1920" height="1080" alt="Cuisine Insights" src="https://github.com/user-attachments/assets/6928c857-c050-470a-b4db-f6d12092dfb1" />

**4. Pricing Analysis**

**Purpose:**
To Analyze how pricing varies by location and how Customer Preference varies.

**Includes**

- Average Ratings By Votes and Cost
- Priciest Restaurant Distribution By Location
- Price and Vote Relationship In Priciest Locations

<img width="1920" height="1080" alt="Pricing Analysis" src="https://github.com/user-attachments/assets/e87759b4-3ecb-4faa-b1a0-1648ed9d7a56" />

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
- A strong relationship cannot be developed between Ratings and Votes.
- We can see that as the cost of the food increases, ratings generally tend to increase. Also after a certain threshold of food price which is like 1500-1700, most ratings are in the range of 4+ which
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








