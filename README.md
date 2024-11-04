# California Employment Statistics Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Recommendations](#recommendations)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis-eda)
- [Data Analysis](#data-analysis)
- [Key Findings and Recommendations](#key-findings)
- [Limitations and References](#limitations)
- [References](#references)
- [Conclusion](#conclusion)

## Project Overview

This data analysis project aims to provide insights into employment trends across various industries in California from 2014 to 2024. By analyzing employment data, we seek to uncover trends, identify regional patterns, assess the impact of seasonality, and highlight industries experiencing significant growth or decline. Our findings are intended to inform workforce development initiatives and policy recommendations.

## Visualizations

Our visualizations include bar plots, heatmaps, and line charts to effectively illustrate employment trends, grwth rates, and seasonal patterns across California.

## Data Sources

-	Current Employment Statistics Data: The primary dataset used in this analysis is the "ces_2014-2024_monthly_2024419.csv," which contains monthly employment data provided by the California Employment Development Department. This dataset includes industry-specific employment figures, seasonally adjusted metrics, and region-specific data for comprehensive insights.

## Tools

- Excel - Data Cleaning
- MySQL Server - Data Storage and Quering
- Tableau - Data Visualization and Dashboard Creation

## Data Cleaning/Preparation

In the initial data preparation phase, we performed several steps to ensure accuracy and consistency:
1. Data loading and inspection: loaded data into MySQL and Tableau for seamless analysis.
2. Data Cleaning: Addressed missing values, filtered out not relevant rows, and standardized date formats
3. Column Creation: Added columns for California State location, and relevant categories for enhanced filtering.

## Exploratory Data Analysis (EDA)

During EDA, we explored the data to address key questions, such as:
- Employment Trends Over Time: How has employment changed across industries over the years?
- Regional Patterns: What are the employment trends across different area types (e.g., metropolitan vs. non-metropolitan)?
- Seasonal Employment Patterns: How does seasonally adjusted employment compare to non-adjusted figures over time?
- Industry Growth: Which industries have experienced the highest growth or decline?

## Data Analysis

In the analysis phase, we utilized SQL queries and Python with Pandas for data manipulation and to derive insights. Here’s an example SQL query used:
```sql
SELECT Industry_Title, Year, AVG(Current_Employment) as Avg_Employment
FROM ces_data
WHERE State = 'California'
GROUP BY Industry_Title, Year
ORDER BY Avg_Employment DESC;
```
## Key Findings

Key findings from the analysis include:
1. Employment Growth: Several industries, particularly those in tech and healthcare, have shown consistent employment growth, while others faced declines.
3. Seasonality Impact: Seasonally adjusted employment data reveal that certain industries experience recurring fluctuations, likely tied to specific times of the year.
4. Top-Performing Regions: Metropolitan areas consistently report higher employment rates, though certain rural areas show rapid growth in specific industries.

## Recommendations

Based on these findings the following recommendations can help support sustained employment growth and stability in California:
#### 1. Targeted support for Declining Sectors:
  Implement policies or workforce development programs aimed at stabilizing industries showing reduced growth, such as manufacturing.
#### 2.	Investment in High-Growth Industries:
  Continue supporting industries with strong growth potential, particularly in tech and healthcare, to sustain California’s competitive edge.
#### 3.	Regional Development Programs:
  Encourage investment in rural and underserved areas to balance growth across the state and reduce dependency on major metropolitan regions.


## Limitations

This analysis is based on available data up to May 2024, which may limit the insights on recent trends and emerging issues. Additional data and future analyses could provide a more comprehensive understanding of the factors influencing employment in California.

## Conclusion
The analysis provides a clear understanding of how casual riders and annual members differ in their usage of Cyclistic's bike-share service. By targeting specific user behaviors and preferences, Cyclistic can effectively convert more casual riders into loyal annual members, ensureing sustained growth and profitability.

## References

- California Employment Development Department: Primary dataset source.
- U.S. Bureau of Labor Statistics: Comparative industry growth metrics.

## Final Thoughts

This project demonstrates the power of data analysis for uncovering actionable insights into employment trends. By tracking industry, regional, and seasonal trends, California can better anticipate and respond to economic shifts, ultimately supporting a resilient workforce and a thriving economy.

## [Go back to my Webpage](https://JoseAGonzalezR.github.io/Jose_AGonzalez.github.io/)
