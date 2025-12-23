Do Richer Countries Have Happier Citizens?

Analyzing GDP, Minimum Wage, and Happiness in 2024

Contributors
Jeff Li:

Data cleaning, data integration, analysis, visualization, interpretation of results

Elin Na:

Data collection, data quality assessment, documentation, ethical and legal review, reproducibility

Contribution Statement:
Both contributors worked collaboratively throughout the duration of the project. Responsibilities were divided to ensure that all major components of the data lifecycle were addressed, from data acquisition and cleaning to analysis, interpretation, and documentation. Individual roles are listed above to clearly demonstrate how each contributor participated in the project, in accordance with the grading guidelines.

Summary
People often assume that countries with higher levels of wealth are happier places to live. Measures such as Gross Domestic Product (GDP) and wages are frequently used by governments and international organizations to evaluate national success and progress. Higher income levels are commonly associated with better access to resources, improved infrastructure, and higher standards of living. However, happiness is a complex concept that extends beyond economic output alone. Individuals’ wellbeing is also shaped by social relationships, health, personal freedom, and trust in institutions. As a result, higher national income does not necessarily guarantee that people feel satisfied, secure, or fulfilled in their daily lives.

This project explores whether richer countries are actually happier and examines whether economic indicators such as GDP and national minimum wage explain happiness better than social and health-related factors. Our central research question is whether higher GDP and higher minimum wages are associated with higher national happiness scores, and how these economic measures compare to non-economic variables such as social support, healthy life expectancy, and freedom to make life choices. We hypothesize that while economic factors may show some relationship with happiness, social and health indicators will be stronger predictors once multiple factors are considered simultaneously.

To investigate this question, we combined two publicly available datasets. The first dataset comes from the World Happiness Report 2024, which is based on survey responses collected through the Gallup World Poll. Respondents in each country are asked to evaluate their overall life satisfaction using a ladder scale ranging from zero to ten, where higher values indicate greater happiness. In addition to the happiness score, this dataset includes explanatory variables such as social support, healthy life expectancy, freedom to make life choices, generosity, and perceptions of corruption. These measures capture aspects of wellbeing that go beyond income and economic production.

The second dataset, Countries of the World 2023, provides economic and demographic information compiled from sources such as the World Bank and the United Nations. From this dataset, we focused on variables including GDP, national minimum wage, population size, unemployment rate, labor force participation, and life expectancy. These indicators describe a country’s economic conditions and labor market structure and allow for comparison across nations.

Before analysis, both datasets were cleaned separately. This process involved removing rows with missing key variables, standardizing country names to ensure consistency across datasets, and converting numeric values that were stored as text into proper numerical formats. After cleaning, the datasets were merged using the country name as the key. The merged dataset initially contained 115 countries. Because national minimum wage is central to our research question, we excluded 21 countries that do not have a nationally defined minimum wage. These countries often rely on collective bargaining systems, which are difficult to compare directly with statutory minimum wages. The final dataset used for analysis includes 94 countries.

We analyzed the data using correlation analysis and multiple linear regression. Correlation analysis allowed us to examine pairwise relationships between happiness and individual variables, while regression analysis enabled us to evaluate how multiple factors jointly explain differences in happiness across countries. Our results indicate that GDP alone has only a weak relationship with happiness. When social support, health, freedom, and minimum wage are included in the regression model, GDP is no longer a statistically significant predictor of happiness.

Instead, social and health-related factors play a much larger role in explaining national happiness levels. Countries with stronger social support networks, longer healthy life expectancy, greater freedom in daily life, and higher minimum wages tend to report higher happiness scores. These findings suggest that economic growth alone does not guarantee improved wellbeing unless economic resources translate into better social conditions and quality of life.

Overall, this project demonstrates the importance of looking beyond traditional economic measures when evaluating national success. Policymakers who focus solely on increasing GDP may overlook key drivers of happiness and wellbeing. Our analysis highlights the value of social support systems, health outcomes, and labor protections in promoting happier societies.

Data Profile
This project uses two publicly available datasets obtained from Kaggle. Both datasets report information at the country level and do not include individual-level or personally identifiable data. As a result, they are suitable for comparative analysis while posing minimal ethical or privacy risks.

The World Happiness Report 2024 dataset is based on survey data collected through the Gallup World Poll. Gallup uses nationally representative samples and standardized survey methods to measure how individuals evaluate their overall quality of life. Respondents are asked to imagine a ladder with steps numbered from zero to ten, where zero represents the worst possible life and ten represents the best possible life. They are then asked to place themselves on this ladder. The average score for each country is reported as the national happiness score.

In addition to the happiness score, the dataset includes several explanatory variables that are commonly associated with wellbeing. These include social support, which reflects whether individuals feel they have someone to rely on in times of need; healthy life expectancy, which measures expected years of life in good health; freedom to make life choices; generosity; and perceptions of corruption. These variables help contextualize happiness by capturing non-economic aspects of quality of life.

All values in this dataset are aggregated at the country level, and no personal identifiers are included. The dataset represents a single year and is designed for cross-country comparisons rather than longitudinal analysis. While happiness surveys can be subjective and influenced by cultural norms, the World Happiness Report is widely used in academic research and policy discussions.

The Countries of the World 2023 dataset combines economic and demographic data from reputable international organizations such as the World Bank, the United Nations, and the International Labour Organization. For this project, we used variables including GDP, national minimum wage, population size, unemployment rate, labor force participation, and life expectancy.

These variables provide insight into a country’s economic capacity and labor market conditions. GDP serves as a broad measure of economic output, while minimum wage reflects labor policy and income protection for workers. Like the happiness dataset, all values are reported at the country level and do not include individual records.

One limitation of this dataset is that minimum wage definitions vary across countries, and some countries do not have a nationally defined minimum wage. This limitation influenced our data cleaning and analysis decisions.

Both datasets are publicly available on Kaggle and are permitted for educational and research use under Kaggle’s terms of service.

Ethics & Legal Constraints
This project uses published datasets which are all licensed for educational and research purposes under the Kaggle website. The datasets include important details about countries and territories that were listed here. The World Happiness Report 2024 is released within the CC0 Public Domain which means that it can be used freely for anyone without any limitations or restrictions. The Countries of the World 2023 dataset is licensed and distributed under Attribution 4.0 International (CC BY 4.0). This specifically requires appropriate credit to the original data source unlike the World Happiness Report 2024. All of the citations and attributions are listed and cited in the References section under this project report. 
Since the analysis for this project relies entirely on aggregated national-level statistics, there is little to no privacy concerns when it comes to the respondents. The Gallup World Poll has established ethical protocols and rules when it comes to conducting survey research which requires consent and must be a voluntary participation. However, it is very important to understand that for aggregated data, it can obscure significant within-country variation. Since there are national averages, they may hide inequalities across multiple regions, demographic populations, and income groups. For example, even though a country may have a high happiness report, there are still communities within that country that face hardship. With our analysis, it does not really entirely capture the disparities and inequalities. Therefore, users should be extremely careful and mindful about generalizing findings and understand that not all generalized findings are factually correct to all people within a country. 
The datasets that were used for this research project were all compiled by reputable global organizations such as The United Nations, the International Labour Organization, and the World Bank. These institutions maintain advanced data collection standards and all of their methodologies are publicly updated and published. However, there are also challenges that come along with using the datasets that we used. If there were surveys, their questions may be approached differently across different people in different countries and different cultures. For example, there may be differences in how each country measures or defines unemployment or labor force participation. With these inconsistencies, it would unintentionally introduce bias and hinder our preciseness in our research findings. While we are attempting to use standardized variables, data users need to be wary that cultural differences and how the country is run may impact the results of the data. 
Additionally, another ethical consideration that is important for this project involves cleaning out countries that did not have defined minimum wages. Twenty-one countries were removed from our analysis and project because they did not have a reported minimum wage, and often relied on sector-specific agreements instead. Because we excluded the twenty-one countries, this exclusion may introduce selection bias, since countries that follow a more collective bargaining system have different rules and regulations when it comes to the topic and issue of the minimum wage system. We did not exclude them out of spite, but the decision for this was due to avoid introducing artificial relationships and providing false information for users. We need to remain transparent to gain the public's trust. However, since we made this difficult decision, our overall findings and results do not generalize all of the existing economic systems and users should interpret the results within these limitations.
Lastly, even though the goal of this project is to contribute to policy discussions regarding economic development and well being, correlation does not imply causation. Although our results point to correlations between happiness and a number of social and economic variables, they do not prove that changes in one variable directly influence changes in another. Instead of viewing these findings as conclusive proof for particular interventions, policymakers should view them as descriptive insights. To use this research responsibly, one must be aware of its limitations, scope, and the situations in which its conclusions might or might not be applicable. 
Data Quality
We conducted a thorough data quality assessment before integrating and analyzing the datasets to ensure that the results of our analysis were reliable, transparent, and reproducible. Because this project combines data from two different sources, careful attention to completeness, consistency, and formatting was essential in order to avoid misleading conclusions.

For the World Happiness dataset, most countries had complete information across all variables of interest, including happiness score, social support, healthy life expectancy, and freedom to make life choices. One country, Tajikistan, was missing several key happiness-related variables and could not be meaningfully included in the analysis. Because these missing values affected the dependent variable itself, Tajikistan was removed from the dataset entirely. Afghanistan reported an extremely low happiness score relative to other countries. However, this value reflects real-world social and political conditions rather than a data entry error or measurement problem. For this reason, Afghanistan was retained in the dataset and treated as a meaningful outlier rather than being removed or adjusted.

In the Countries of the World dataset, the primary data quality issue involved missing minimum wage values. Twenty-one countries did not report a nationally defined minimum wage. In many cases, these countries rely on collective bargaining systems or sector-specific wage agreements rather than a single statutory minimum wage. Because minimum wage is central to our research question, we chose not to estimate or impute these missing values. Imputation would require strong assumptions about labor markets and wage-setting mechanisms that vary significantly across countries and could introduce bias or artificial relationships. Instead, these countries were excluded from the analysis to preserve methodological clarity and comparability.

Several variables, including GDP and minimum wage, were originally stored as text strings containing currency symbols, commas, or other non-numeric characters. These formatting issues prevented the variables from being used directly in calculations and statistical models. We addressed this problem by systematically cleaning each variable, removing non-numeric characters, and converting the values into numeric data types. This step was essential for ensuring accurate correlation and regression analysis.

Missing or blank cells were handled consistently across both datasets. Rows with missing values in key variables were removed rather than filled in with estimated values. While this approach reduces the overall sample size, it avoids introducing uncertainty from imputed data and ensures that all observations used in the analysis are based on reported values. Country names differed slightly between datasets, which posed a risk of incorrect merging. These discrepancies were resolved manually by standardizing country names to ensure accurate alignment. Territories and regions that were not sovereign countries were removed to maintain consistency across datasets.

After cleaning and integration, the final dataset contains 94 countries and has no missing values in the variables used for analysis. All variables are numeric, consistently formatted, and directly comparable across countries. Although excluding countries without minimum wage data may introduce some selection bias, this decision was necessary to ensure meaningful comparisons and to maintain transparency about the limitations of the analysis.

Findings
The results of this project indicate that happiness is more closely associated with social and health-related factors than with economic output alone. While economic measures such as GDP and minimum wage are often assumed to be strong indicators of wellbeing, our analysis shows that they do not fully explain differences in happiness across countries.

Correlation analysis reveals strong positive relationships between happiness and social support, healthy life expectancy, freedom to make life choices, and minimum wage. Countries with stronger social networks and better health outcomes tend to report higher happiness scores. In contrast, GDP shows only a weak correlation with happiness. This suggests that economic size alone does not capture the factors that contribute most directly to people’s life satisfaction.

To further examine how these variables interact, we used a multiple linear regression model with happiness score as the dependent variable. The model includes GDP, minimum wage, social support, healthy life expectancy, and freedom as independent variables. The regression explains over eighty percent of the variation in happiness scores across countries, indicating a strong overall fit and suggesting that the included variables capture most of the factors influencing national happiness.

The regression results show that social support, freedom to make life choices, minimum wage, and healthy life expectancy are all statistically significant predictors of happiness. Each of these variables has a positive relationship with happiness, meaning that higher values are associated with higher reported life satisfaction. GDP, however, is not statistically significant once these other factors are included in the model.

This finding suggests that GDP’s apparent relationship with happiness is largely indirect. Wealth may contribute to happiness only insofar as it enables better health outcomes, stronger social safety nets, and greater individual freedom. When these conditions are accounted for explicitly, GDP itself does not add explanatory power. In practical terms, this means that simply increasing economic output does not guarantee higher happiness unless the benefits of growth are translated into improvements in daily life.

These results have important implications for policy and evaluation. Governments that focus exclusively on economic growth may overlook key drivers of wellbeing. Investments in healthcare, social support systems, and labor protections such as minimum wage policies appear to play a more direct role in promoting happiness. The visualizations included in the results folder, such as correlation heatmaps and scatter plots, support these conclusions by illustrating the relative strength of different relationships.

Overall, the findings reinforce the idea that happiness is multidimensional. Economic indicators matter, but social and health-related factors are more central to how people evaluate their lives.

Future Work
There are several ways this project could be expanded and improved in future work. One important extension would be to incorporate data from multiple years rather than focusing on a single snapshot in time. A longitudinal analysis would allow researchers to examine how changes in economic conditions, labor policies, and social factors affect happiness over time. By observing trends rather than single-year comparisons, future studies could better distinguish between short-term fluctuations and long-term structural relationships. This approach would also allow for stronger conclusions about causality rather than simple correlation, helping determine whether changes in policy or economic conditions actually lead to measurable changes in happiness.

Future research could also include measures of inequality, such as income distribution, poverty rates, or cost of living indices. National averages may hide important disparities within countries, particularly in nations with large income gaps or regional differences. It is possible for a country to report high average happiness while certain populations experience significantly lower wellbeing. Including inequality-related variables would provide a more nuanced understanding of how economic and social conditions affect different groups and would help clarify whether economic growth benefits are shared broadly across society.

Another promising direction would be to examine specific policy changes in greater detail. For example, researchers could study the effects of minimum wage increases, healthcare reforms, or expansions of social welfare programs on happiness outcomes. Comparing countries before and after major policy implementations, or using quasi-experimental designs where possible, could help isolate the impact of these interventions. This type of analysis would be especially valuable for policymakers seeking evidence-based guidance on which policies most effectively improve quality of life. Similarly, incorporating cultural and political variables such as trust in government, political stability, or civic engagement could shed light on how institutional environments shape happiness beyond economic conditions alone.

From a methodological perspective, future work could explore alternative modeling approaches. While this project relied on correlation analysis and linear regression, more advanced techniques could capture complex relationships between variables. Nonlinear models, interaction terms, or hierarchical models might reveal that the impact of one variable depends on another, such as minimum wage having a stronger effect in countries with higher costs of living or stronger labor protections. Exploring these interactions could yield deeper insights into the mechanisms linking economic and social factors to happiness.

From a technical standpoint, the workflow could be further automated to improve reproducibility and efficiency. Tools such as Snakemake or Make could be used to create an end-to-end pipeline that runs data acquisition, cleaning, integration, analysis, and visualization with a single command. Additional documentation, clearer file organization, and more detailed comments within scripts would also make the project easier for others to understand and reuse. Expanding the set of visualizations and providing interactive plots could further enhance accessibility and interpretability.

Overall, this project provides a strong foundation for examining the relationship between economic conditions and happiness, but there remains significant potential for deeper analysis, broader scope, and more robust causal investigation in future research.


Reproducing
Clone the repository and create a Python environment.
Install required dependencies listed in the requirements.txt file.
Download the raw datasets from kaggle.
World Happiness Report - 2024
Global Country Information Dataset
Place the files in the project root directory.
Run the analysis script or notebook from start to finish.
Output files will be generated in the data and results directories as specified.

References
Datasets
Singh, A. (2024, March 31). World happiness report 2024. Kaggle. https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2024 
Elgiriyewithana, N. (2023, July 8). Global Country Information Dataset 2023. Kaggle. https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023 

Software & Code
Kaggle Team. (2025, June 22). Terms of use. Kaggle. https://www.kaggle.com/terms 
Harris, C.R., Millman, K.J., van der Walt, S.J. et al. Array programming with NumPy. Nature 585, 357–362 (2020). DOI: 10.1038/s41586-020-2649-2.
pandas development team. (2024). pandas (v2.2.2). https://pandas.pydata.org
Python Software Foundation. (2024). Python (v3.12) [Computer software]. https://www.python.org/

Licenses
Data is used according to the licenses provided by the original Kaggle datasets.
All original code in this repository is released under the MIT License unless otherwise stated.

