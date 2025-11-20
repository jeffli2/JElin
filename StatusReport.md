### Data Cleaning (Elin)
- [World Data 2023](world-data-2023-(1)-csv-csv.csv)
- [Happiness Report 2024](World-happiness-report-2024-csv-csv.csv)

### Data Integration Code (Jeff)
- [Data Integration Notebook](DataIntegration.ipynb)

Status Report
Our Mission:
As previously mentioned, we are trying to figure out whether richer countries with citizens earning higher minimum wages are happier than those who are in poorer countries. To do this, we are using two unique datasets. One of the datasets shows the happiness reports from around the world, and the other dataset displays more of the income and GDP reports.
Updates:
October 10 (Completed)
We found and downloaded two datasets from Kaggle. The first one contains happiness ratings for different countries, while the second one has economic information like GDP and minimum wage. Both datasets had most of the information we needed to begin our analysis.
October 19 (Completed)
We cleaned both datasets individually prior to integration. For fair comparison, we standardized country names to uppercase, converted all minimum wages to US dollars for fair comparison, and found data quality issues in every dataset.
For the World Data 2023 dataset, we removed 21 countries that had missing values in key variables. For the Happiness Report 2024 dataset, we removed 1 country (Tajikistan) that was missing critical happiness metrics. We also found Afghanistan as a statistical outlier with an unusually low happiness score (1.721).
October 24 (Completed)
Jeff combined the two cleaned datasets based on the names of the countries. This process required handling name mismatches; for example, "Czechia" needed to be standardized to "Czech Republic," "Turkiye" to "Turkey," and "Taiwan Province of China" to "Taiwan." Jeff fixed 6 such mismatches to ensure correct matching.
After the integration, Jeff was able to combine 115 countries with comprehensive data from both datasets. The final integrated dataset contains 27 variables combining economic indicators (GDP, minimum wage, unemployment, population) with happiness metrics (happiness score, social support, freedom, life expectancy).
Jeff found that there are no minimum wage laws in 21 of the countries in our integrated dataset. It's interesting to note that many of these are highly developed nations like Denmark, Sweden, Norway, Finland, and Iceland, which use collective bargaining instead of statutory minimum wages.
November 8 (Completed)
Jeff ran statistical tests to determine whether there is actually a correlation between minimum wage, happiness, and overall GDP. We found that life expectancy (correlation: 0.744) and freedom (correlation: 0.642) are much stronger predictors of happiness than GDP alone (correlation: 0.165). Additionally, we developed regression models to examine the relationship between GDP and minimum wage and happiness, and we have recorded the outcomes.
November 12 (Completed)
On November 12, Elin had finished creating scripts that can run the entire analysis automatically. With this, any user can run the entire project with a simple command instead of doing it manually and step-by-step, which is very tedious.
November 14 (Still kind of in progress, will be completed by Nov 21)
In order for other users to replicate our analysis, Jeff is still working to complete the instructions. We have compiled a list of the necessary software and packages as a team, and we are currently editing and refining the detailed instructions that outline how to set everything up.
November 16 (Still kind of in progress, will be completed by Nov 22)
We are still working on providing thorough explanations of the variables in our data as well as the meanings of the data's columns. This will make it easier for researchers and data scientists to comprehend our methodology and strategy for utilizing our data.
Timeline:
October 10: We wanted to focus on our project based on countries and their reports. With this, we kicked it off by finding and downloading the two datasets from the Kaggle website. This was a very successful, and not lengthy process.
October 18-19: These days, we cleaned the two datasets independently. We eliminated 21 nations from the World Data and 1 from the Happiness Report that had missing values. Additionally, we converted all minimum wages to US dollars and standardized country names to uppercase. Prior to integration, the data was thoroughly cleaned to guarantee its quality.
October 24: Jeff combined the cleaned datasets together. The main challenges were handling name mismatches (like "Czechia" vs "Czech Republic") and ensuring only countries with complete data were included. After fixing 6 name mismatches, Jeff successfully integrated 115 countries.
November 1-15: Through this time period, Jeff worked on statistical analysis. The analysis took quite a bit of time and effort, and there were some deadline delays due to the lengthy process. However, Jeff finally finished by November 15.
November 1-16: In this time period, Elin was working on the automated pipeline and finally finished by November 16, which was our deadline.
November 1-17 (now): Jeff is working on writing the documentation regarding reproducibility in this time period. Jeff is almost done, and Elin is pitching in to assist.
November 17-20 (this week): We are trying to finish and polish up the metadata documentation as well as testing/training the reproducibility.
November 21-25 (next week): This is the week where we proofread everything and make sure that everything is as perfect and precise as possible. Since it is during fall break, we might have some delays.
Changes:
As we progressed, we made  a few changes. The statistical analysis took longer than our original October 17 deadline, but we finished it by November 15. This extra time was worth it because we found some interesting patterns in the data that we explored carefully with better statistical models.
We also decided to have both of us work on different tasks at the same time instead of one after another. This saved us time and helped us finish the analysis and automation earlier than expected. We added some extra automation tools (GitHub Actions) that weren't in our original plan to make the project easier to reproduce.
The data cleaning took more time than we thought. We originally planned one day, but it took until October 24 because we had to be thorough about removing countries with missing values, standardizing country names across both datasets, handling name mismatches, and converting different currencies to US dollars.
Rather than attempting to impute or estimate the data, we simply eliminated any nations with missing values. This guaranteed that all 27 variables in our final integrated dataset of 115 countries had accurate and comprehensive data.
Our Contributions:
Jeff's Contributions
During this milestone and throughout the project, I focused on data integration and making the project reproducible. I performed the data integration by merging the two cleaned datasets, handling country name mismatches, and creating the final integrated dataset with 115 countries and 27 variables. I also set up virtual environments and wrote installation instructions for reproducibility. Additionally, I assisted Elin with tasks related to data extraction. Together, I have spent about 15 hours on this milestone.
Elin's Contributions
I worked on data cleaning and statistical analysis during this milestone. It was my responsibility to clean each dataset separately by standardizing formats and eliminating nations with missing values. For the project, I also wrote automation scripts and ran the regression models. During all of these times, I worked for 15 hours.
