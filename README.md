# Inflation Impact Analysis

## Overview
Inflation occurs when there is a sustained increase in the general price level of goods and services in an economy over time. It impacts various aspects of the economy, including purchasing power, consumer behaviour, savings, and investment. Moderate inflation is typically a sign of a healthy, growing economy, as it encourages spending and investment. However, high or unpredictable inflation can erode the value of money, disrupt financial planning, and lead to economic uncertainty.

To analyze the impact of inflation, I need to compare it with other economic indicators. So, to analyze the impact of inflation on the economy, I will compare it with the exchange rates over time. This comparison is important because exchange rates are influenced by inflation differentials between countries, such that higher inflation in a country generally leads to a weaker currency relative to countries with lower inflation.

## Inflation Impact Analysis with Python
I have two data files for this task. Let’s start the task of inflation impact analysis by importing the necessary Python libraries and the [datasets](https://statso.io/impact-of-inflation-case-study/).

I will now prepare this dataset for analysis by merging the relevant parts of these datasets to analyze the impact of inflation on exchange rates.

The merged dataset now contains the following columns for each year:
- **Exchange Rate (INR/USD):** The average exchange rate of INR to USD.
- **Inflation Rate (India):** The inflation rate for India.
- **Inflation Rate (United States):** The inflation rate for the United States.

Let’s start by analyzing the trend of inflation rates for both India and the United States alongside the exchange rate:

![Trend Analysis](https://github.com/Sourabh1710/Inflation-Impact-Analysis/blob/main/images/Trends%20of%20Exchange%20Rate%20and%20Inflation%20Rates.png)  

The exchange rate shows a general upward trend over the years, which indicates a depreciation of the Indian Rupee against the US Dollar. However, there are periods of both sharp increases and relative stability.

India’s inflation rate has fluctuated significantly over the years, with periods of high inflation (e.g., early 2000s) and more stable inflation in recent years. The United States has generally experienced lower and more stable inflation rates compared to India, with fewer extreme fluctuations.

## Correlation Analysis
Next, I will perform a correlation analysis to explore the relationship between the inflation rates and the exchange rates.

### Findings from the correlation analysis:
- **Exchange Rate vs. Inflation Rate (India):** The correlation coefficient is approximately -0.34, which indicates a weak negative relationship. It suggests that as inflation in India increases, the INR tends to depreciate against the USD, though the relationship is not very strong.
- **Exchange Rate vs. Inflation Rate (United States):** The correlation coefficient is approximately 0.24, which indicates a weak positive relationship. It suggests that higher inflation in the United States might be associated with a depreciation of the USD against the INR, but again, the relationship is not strong.
- **Inflation Rate (India) vs. Inflation Rate (United States):** The correlation between the inflation rates of India and the United States is very weak and negative (-0.12), which indicates that the inflation rates in these two countries do not move together.

## Comparative Analysis
Next, I will perform a comparative analysis to highlight periods of significant divergence or convergence between the inflation rates and the exchange rates:

![Comparative Analysis](https://github.com/Sourabh1710/Inflation-Impact-Analysis/blob/main/images/Comparative%20Analysis-%20Exchange%20Rate%20vs%20Inflation%20Rates%20(India%20and%20US).png)  

### Findings from the comparative analysis:
- **Early 2000s:** A period of high inflation in India coincides with a period of relative stability in the exchange rate. It suggests that factors other than inflation may have been driving the exchange rate during this time.
- **Late 2000s to Early 2010s:** The period shows some alignment between rising inflation in India and a weakening INR, which indicates that inflation could be contributing to exchange rate movements.
- **2015 Onwards:** The exchange rate continues to rise, while both India’s and the United States’ inflation rates remain relatively low. This divergence suggests that the exchange rate is influenced by additional factors beyond inflation, such as economic growth, monetary policy, and international trade dynamics.

## Analyzing Inflation based on the Purchasing Power Parity (PPP)
Purchasing Power Parity (PPP) is an economic theory that suggests that in the long term, exchange rates between two countries should adjust so that a basket of goods costs the same in both countries when priced in a common currency. PPP is used as a method to compare the economic productivity and standards of living between different countries. If one country’s inflation rate is higher than another’s, its currency should depreciate accordingly to maintain parity in purchasing power to ensure that the same goods cost the same in both locations.

I will now analyze whether the Purchasing Power Parity theory holds by comparing the relative inflation rates and exchange rate movements over time. It will provide a deeper understanding of whether the exchange rate aligns with the theoretical value based on inflation differentials.

To test whether PPP holds for India and the United States, I can:

- **Calculate the Expected Exchange Rate Based on PPP**
- **Compare the Actual Exchange Rate with the PPP-Based Expected Exchange Rate**

The formula for PPP-based exchange rate prediction is:

\[\text{Expected Exchange Rate} = \text{Initial Exchange Rate} \times \left( \frac{1 + \text{Inflation Rate in India}}{1 + \text{Inflation Rate in the US}} \right)\]

Let’s calculate and visualize the PPP-based expected exchange rate versus the actual exchange rate:

![PPP Analysis](https://github.com/Sourabh1710/Inflation-Impact-Analysis/blob/main/images/Actual%20vs.%20Expected%20Exchange%20Rate%20(PPP).png)  

The blue line represents the actual exchange rate (INR/USD) over time, while the orange dashed line represents the expected exchange rate based on PPP. In some periods, the actual exchange rate closely follows the expected PPP-based rate, which suggests that PPP holds. However, in other periods, there are significant deviations between the two.

The PPP-based expected exchange rate shows a more rapid increase compared to the actual exchange rate. It suggests that, according to PPP, the INR should have depreciated more than it actually did. However, the actual exchange rate was consistently lower than the PPP-based expected rate, which indicates that factors other than inflation are at play.

## Conclusion
My analysis revealed that inflation in India and the United States influences the exchange rate between INR and USD. Higher inflation in India generally leads to a depreciation of the INR relative to the USD, while lower inflation in the United States contributes to a stronger USD. While inflation affects the exchange rate between INR and USD, it is only one of many factors.

---
## Author
Sourabh Sonker <br>
Data Scientist
