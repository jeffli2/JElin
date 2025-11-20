### Data Cleaning (Elin)
- [World Data 2023](world-data-2023-(1)-csv-csv.csv)
- [Happiness Report 2024](World-happiness-report-2024-csv-csv.csv)

### Data Integration Code (Jeff)
- [Data Integration Notebook](DataIntegration.ipynb)

Status Report
Our Mission:

As mentioned previously, we are trying to determine whether if the richer countries with people earning better minimum wages are happier than citizens who live in poorer countries like those in Africa. 

To do this, we are using two unique datasets.
One of the datasets shows the happiness reports from around the world, and the other dataset displays more of the income and GDP reports.

Updates:
October 10 (Completed)

We found and downloaded two datasets from Kaggle. The first dataset contains happiness ratings for the listed countries, and the second dataset includes more economic and finance related information like minimum wage and overall GDP.
Both datasets had most of the information we needed to begin our analysis.

October 19 (Completed)

From the World Data dataset, Jeff had removed 21 countries that had missing values that may alter the results of the data.
For the Happiness Report 2024 dataset, we removed 1 country (Tajikistan) that was missing critical happiness metrics. We also found Afghanistan as a statistical outlier with an unusually low happiness score (1.721).

October 24 (Completed)

Jeff combined the two cleaned datasets based on the names of the countries. This process required Getting rid of some "countries" that were not actually countries such as Hong Kong and U.S. territories that are not real countries. This process was relatively easy and not too difficult. 

After integration of the two datasets, Jeff had combined the 115 countries with the provided data from both datasets.
The final integrated dataset contains 27 variables combining economic indicators (GDP, minimum wage, unemployment, population) with happiness metrics (happiness score, social support, freedom, life expectancy).

Jeff found that there are no minimum wage laws in 21 of the countries in our integrated dataset. It's interesting to note that many of these are highly developed nations like Denmark, Sweden, Norway, Finland, and Iceland, which use collective bargaining instead of statutory minimum wages, but since we are only focusing on the minimum wages, we had to clean them out.

November 8 (Completed)

Jeff ran statistical tests to determine whether there is actually a correlation between minimum wage, happiness, and overall GDP. We found that life expectancy (correlation: 0.744) and freedom (correlation: 0.642) are much stronger predictors of happiness than GDP alone (correlation: 0.165).

November 12 (Completed)

On November 12, Elin finished working on cleaning the data, and addressing any odd observations in the datasets.

November 14 (Still kind of in progress, will be completed by Nov 21)

In order for other users to replicate our analysis, Jeff is still working to complete the instructions. We have compiled a list of the necessary software and packages as a team, and we are currently editing and refining the detailed instructions that outline how to set everything up.

November 16 (Still kind of in progress, will be completed by Nov 22)

We are still working on providing thorough explanations of the variables in our data as well as the meanings of the data's columns. This will ensure that our datasets and techniques that we are using is replicable and transparent for different users as well as data scientists and researchers.

Timeline:

October 10: We wanted to focus on our project based on countries and their reports. With this, we kicked it off by finding and downloading the two datasets from the Kaggle website. This was a very successful, and not a lengthy process.

October 18-19: These days, we cleaned the two datasets independently. We eliminated 21 nations from the World Data and 1 from the Happiness Report that had missing values. Additionally, we cleaned out certain countries we do not need or those who have a lot of missing values. Prior to integration, the data was thoroughly cleaned to guarantee its quality.

October 24: Jeff combined the cleaned datasets together. The main challenges were some countries were not officially recognized as countries and there was a country that consisted of emojis so we had to get rid of that, Jeff successfully integrated 115 countries.

November 1-15: Through this time period, Jeff worked on statistical analysis.The analysis definitely took a huge chunk of time and effort, and there were some deadline delays that occured. However, Jeff was able to finish by November 15. Additionally, in this time period, Elin worked on data cleaning to ensure that there will be no errors or any problems with our research goals.

November 1-17 (now): Jeff is working on writing the documentation regarding reproducibility in this time period. Jeff is almost done, and Elin is pitching in to assist.

November 17-20 (this week): We are trying to finish and polish up the metadata documentation as well as testing/training the reproducibility.

November 21-25 (next week): This is the week where we proofread everything and make sure that everything is as perfect and precise as possible.
Since it is during fall break, we might have some delays.

Changes:

As we progressed, we made a few changes. The statistical analysis took longer than our original October 17 deadline, but we finished it by November 15. This extra time was worth it because we found some interesting patterns in the data that we explored carefully with better statistical models.

We also decided to have both of us work on different tasks at the same time instead of one after another.
This saved us time and helped us finish the analysis earlier than expected. We added some extra automation tools (GitHub Actions) that weren't in our original plan to make the project easier to reproduce.

The data cleaning took more time than we thought. We originally planned one day, but it took until October 24 because we had to be thorough about removing countries with missing values, standardizing country names across both datasets, handling name mismatches, and converting different currencies to US dollars.

Rather than attempting to impute or estimate the data, we simply eliminated any nations with missing values. This guaranteed that all 27 variables in our final integrated dataset of 115 countries had accurate and comprehensive data.

Our Contributions:
Jeff's Contributions

During this milestone and throughout the project, I focused on data integration and making the project reproducible. I performed the data integration by merging the two cleaned datasets, and creating the final integrated dataset with 115 countries and 27 variables.
I also set up virtual environments and wrote installation instructions for reproducibility. Additionally, I assisted Elin with tasks related to data extraction. Together, I have spent about 15 hours on this milestone.

Elin's Contributions

I worked on data cleaning during this milestone. It was my responsibility to clean each dataset separately by standardizing formats and eliminating nations with missing values. During all of these times, I worked for 15 hours.
