# Property Evaluation Tool for Residential Real Estate Investors

![image](./Resources/img/housing.png)

# Contributors
### Antonio Garza
### Mike Hobbs
### Ezra Hsiao

---
This tool allows the user to understand potential market oportunities in the real estate markets for single family houses is a comprehensive real estate market analysis solution. This solution enables users to access a vast array of data about each of the 10 in markets, such as historical and current home prices, market trends, rental rates, supply and demand statistics, economic indicators, and population growth rates.

The solution provides users with a user-friendly interface that allows for easy navigation of data and enables users to customize their analysis based on state and city. The tool can generate reports and charts that present the data in a clear and easy-to-understand format, making it easy for users to interpret and draw insights from the data.

The software's data is collected from a variety of sources, including public records, MLS data, economic indicators, and other sources. The tool uses data science to analyze the data.

Overall, this tool is an essential resource for real estate investors, brokers, and other professionals who want to stay on top of the latest trends and make informed decisions about buying, selling, or investing in single-family houses in growing real estate markets.

---

# "Investor In Town" -- Market/Property Evaluation Tool for Residential Real Estate Investors

Often times, real eastate investors may have only a day or two in a city to look at potential investment properties and even less time to research them.  Our project is designed to provide residential real estate investors with a tool that uses calculated metrics to help narrow their search for investment properties based on a set of criteria. These metrics can be both market (city/state) and property based so that investors can start by narrowing from a list of cities, then filter individual properties within that market to determine which rental houses show attractive investment ratios and ultimately, plot their stops on a map.

In this project, we will take a closer look at one of the most popular areas of the United States for residential real estate investors. The United States "Sun Belt" (which includes East Texas and the Southeastern US) has been offering attractive returns to investors over the last several years due to its high population and job growth.  But which cities in the Sun Belt offer the best investment properties, and which properties within those markets should an investor take a closer look at.  "Investor In Town" will answer these questions.

The following 10 cities will be evaluated in this model:

- Dallas, TX
- Austin, TX
- San Antonio, TX
- Houston, TX
- Atlanta, GA
- Charlotte, NC
- Jacksonville, FL
- Tampa, FL
- Orlando, FL
- Miami, FL


## Core Metrics

### We will use a set of core metrics to evaluate and filter data on a market and property level. A list of these metrics can be found below, along with their calculation and goal outcome.

**Market Level**

1. Annual Population Growth by state % (2010 - 2023)

2. Annual Job Growth by state % (2010 - 2023)

3. City Price to Rent Ratio: Median Home Price / Annual Median Rent (monthly rent * 12) 
Goal <= 15

4. Quality of Life Index

5. Cost of Living Index (measure of overall affordability)

6. Housing Price to Income Ratio (measure of housing affordability)


**Property Level**

1. Rent Ratio: Monthly Rent Estimate / Total Cost

Goal >.55%

2. Cap Rate:  Net Operating Income (NOI) / Total Cost

Traditional Rental:  *Goal >= 5%*
AirBNB Rental:  *Goal >= 9.5%*  

## Equations and Variables

# Formulas

1.  Total Cost = List Price + Closing Fees
2.  NOI = Gross Income - Annual Operating Expenses (OpEx)

### Based on the above calculations, we will need to gather the following individual data points (variable and potential source listed below):

1.  Address (Mashvisor API)
2.  City (Mashvisor API)
3.  State (Mashvisor API) 
4.  Zip Code (Mashvisor API)
5.  Latitude (Mashvisor API)
6.  Longitude (Mashvisor API)
7.  List Price (Mashvisor API)
8.  Square Feet (Mashvisor API)
9.  Bed/Bath (Mashvisor API)
10. Estimated Monthly Rent -- Traditional Rental (Mashvisor API)
11. Estimated Monthly Rent -- AirBNB Rental
12. Estimated Net Operating Income (NOI) -- Traditional Rental (Mashvisor API)
13. Estimated Net Operating Income (NOI) -- AirBNB Rental (Mashvisor API)
14. Median Home Price in a given city (Zillow csv: "Zillow Home Value Index")
15. Annual Median Rent in a given city (Zillow csv:  "Zillow Observed Rent Index")
16. Quality of Life Index (Numbeo)