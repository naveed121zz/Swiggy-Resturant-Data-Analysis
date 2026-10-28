# Swiggy Restaurant Data Analysis \| Power BI Dashboard

## About the Project

This project analyzes Swiggy restaurant data using Microsoft Power BI to
explore restaurant distribution, food categories, pricing, customer
ratings, and delivery time. The interactive dashboard helps users
compare cities and areas and identify patterns that can support
data-driven decisions.

## Project Objective

-   Analyze restaurant distribution across cities and areas.
-   Identify the most common food types served by restaurants.
-   Compare average restaurant prices across areas.
-   Understand average ratings and delivery times.
-   Present key metrics and trends in an interactive dashboard.

## Dataset

The dataset contains restaurant-level information, including: - `ID` --
Restaurant record identifier - `Area` -- Area where the restaurant is
listed - `City` -- City in which the restaurant operates - `Restaurant`
-- Restaurant name - `Price` -- Price value recorded in the dataset -
`Avg ratings` -- Average restaurant rating - `Total ratings` -- Total
ratings recorded - `Food type` -- Food categories served - `Address` --
Restaurant address detail - `Delivery time` -- Delivery-time value
recorded in the dataset

*Note: Interpret price and delivery-time units according to the original
dataset's documentation.*

## Tools & Technologies

-   **Microsoft Power BI** -- Dashboard design and interactive analysis
-   **Power Query** -- Data inspection and transformation
-   **DAX** -- Measures and KPI calculations
-   **CSV** -- Source dataset

## Data Cleaning & Transformation

The dataset was reviewed and prepared for analysis in Power BI. Typical
preparation steps for this project include: - Checking column names and
data types. - Reviewing missing or blank values. - Checking for
duplicate records. - Ensuring price, rating, total ratings, and
delivery-time fields use suitable numeric data types. - Standardizing
text fields such as city, area, and food type where required. -
Preparing food-type data for category-level analysis where needed.

*Document only the cleaning steps you actually performed in Power Query;
remove any step that was not part of your workflow.*

## DAX & Measures

The dashboard presents these key metrics: - **Average Rating** --
Average of restaurant ratings. - **Average Price** -- Average of the
price field. - **Restaurant Count** -- Number of restaurant records
included in the analysis. - **Average Delivery Time** -- Average of the
delivery-time field.

Example DAX measures (adjust table and column names to match your Power
BI model):

``` dax
Avg Rating = AVERAGE('Swiggy Data'[Avg ratings])

Avg Price = AVERAGE('Swiggy Data'[Price])

Restaurant Count = DISTINCTCOUNT('Swiggy Data'[ID])

Avg Delivery Time = AVERAGE('Swiggy Data'[Delivery time])
```

## Dashboard Features

-   KPI cards for average rating, average price, restaurant count, and
    average delivery time.
-   Donut chart showing the top five served food types.
-   Bar chart highlighting the top ten areas by restaurant count.
-   Horizontal bar chart comparing average price across selected
    expensive areas.
-   Map visual showing restaurant distribution across cities.
-   Consistent dashboard styling for easier reading and comparison.

## Interactive Filters

-   **City slicer** -- Filter the report by city.
-   **Area slicer** -- Focus on selected areas.
-   Visual interactions allow users to explore how selections affect the
    dashboard metrics and charts.

## Key Business Questions

1.  Which cities have the most restaurant listings?
2.  Which areas have the highest number of restaurants?
3.  What are the most commonly represented food types?
4.  Which areas have the highest average prices?
5.  What is the average restaurant rating?
6.  What is the average delivery time?
7.  How do restaurant patterns vary by city and area?

## Key Insights

The values below are the summary figures displayed in the current
dashboard screenshot. They may change when interactive filters are
applied.

-   **Average Rating:** 3.66
-   **Average Price:** 348.44
-   **Restaurant Records:** 8.68K
-   **Average Delivery Time:** 53.97
-   The donut chart compares the five leading served food-type
    categories.
-   The area ranking highlights Rohini as the leading area in the
    displayed top-ten chart.
-   The price comparison shows Villa Park with the highest displayed
    average-price value among the areas shown.
-   The map supports geographic comparison of restaurant listings across
    cities.

## Project Structure

Suggested GitHub repository structure:

``` text
Swiggy-Restaurant-Data-Analysis/
├── README.md
├── Swiggy Data.csv
├── Dashboard.png
└── swiggy.pbix
```

Keep only the files you choose to publish. If the Power BI file is too
large for GitHub, consider sharing it through an appropriate external
file link instead.

## How to Use

1.  Download or clone this repository.
2.  Open `swiggy.pbix` in Microsoft Power BI Desktop.
3.  If Power BI asks for the dataset location, point the source to
    `Swiggy Data.csv` and refresh the data.
4.  Use the City and Area slicers to explore the dashboard.
5.  Select charts or data points to investigate restaurant distribution,
    food categories, pricing, ratings, and delivery time.

## Skills Demonstrated

-   Data analysis and exploratory data analysis
-   Data cleaning and transformation
-   Power Query
-   DAX measures and KPI development
-   Data visualization and dashboard design
-   Working with CSV datasets
-   Business-question framing and insight communication

## Future Improvements

-   Add trends over time if date-related data becomes available.
-   Include more detailed rating and delivery-time comparisons.
-   Add filters for food type and restaurant.
-   Improve data validation and document missing-value and duplicate
    handling.
-   Add drill-through pages for city- and area-level analysis.
-   Publish the report to Power BI Service where appropriate.

## Conclusion

The Swiggy Restaurant Data Analysis dashboard provides an interactive
overview of restaurant listings, food categories, pricing, ratings, and
delivery times. It demonstrates how Power BI can turn structured
restaurant data into useful visual summaries for exploring business
questions and supporting data-informed decisions.
