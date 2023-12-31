<html>
<h1 style="text-align:left;font-size:150%">Table of Contents : </h1>
</html>


* [Getting started](#sec1)
    * [Importing library](#sec1.1)
    * [Importing dataset](#sec1.2)
    * [Quick overview about data](#sec1.3)
    * [Check Null](#sec1.4)
    * [Check for missing data and data types](#sec1.5)
    * [Check Duplicate](#sec1.6)
    
         
* [Analysis of statistic distribution](#sec2)
  * [Calculate basic statistics for numerical columns](#sec2.1)
  * [Generate summary statistics for categorical columns](#sec2.2)
  * [Explore the relationships between variables using appropriate EDA techniques such as correlation analysis .](#sec2.3)
    * [Heatmap of correlation matrix](#sec2.3.1)
  
* [Analysis of statistic distribution](#sec3)
  * [A histogram to visualize the distribution of a numerical variable.](#sec3.1)
  * [ Bar plot for 'quality' column](#sec3.2)
  * [ Distribution of Quality](#sec3.3)
  * [ Pairplot](#sec3.4)
  * [ Box plot for each continuous variable](#sec3.5)
  * [ Box plot for each continuous variable in dependance of target column](#sec3.6)
  
  
* [Conclusion](#sec4)

**Report - Wine Data**

**Introduction:**
This report focuses on the analysis of a dataset related to wine, including attributes such as fixed acidity, volatile acidity, citric acid, residual sugar, chloride, free sulfur dioxide, density, pH, sulphates, alcohol, quality, and several other attributes. Below is a summary of the findings after data wrangling, exploratory data analysis (EDA), and visualizations.

**1. Data Inspection and Preprocessing:**
- The raw data appeared to be clean, with no significant missing values or obvious errors in the given columns.
- During preprocessing, there was little need for data cleaning.

**2. Data Distribution:**
- The dataset contains both continuous and categorical attributes, with 'quality' as the target variable. 'Quality' is a categorical variable representing the quality of wine on a scale from 3 to 9.
- The distribution of wine quality shows signs of skewness, with a high concentration of wines having quality around 5 and 6.

**3. Data Visualization:**
- Visualizations such as frequency plots, box plots, and scatter plots were created to explore the distribution and relationships between attributes and wine quality.
- Notable findings include a potential relationship between alcohol content and wine quality, as well as the influence of certain chemical attributes (e.g., volatile acidity, citric acid, and sulphates) on wine quality.

**4. Feature Engineering Techniques:**
- Additional feature engineering may be required to better understand the relationships between attributes and wine quality. For example, creating new features or normalizing data for modeling purposes.

**5. Modeling:**
- After completing data preprocessing and exploratory data analysis, the next steps typically involve building predictive models to understand the key factors influencing wine quality.

**6. Conclusion:**
<html>
This project has provided a foundation for in-depth analysis and modeling, allowing you to identify the key factors that influence wine quality and make predictions based on this information. Subsequent steps may include building predictive models to provide quality predictions based on chemical and mechanical attributes.


This dataset shows the rating of >1000 different wines and their chemical parameters. The dataset is unbalanced regarding the different quality ratings. >80 % of the wines get a rating of "5" or "6" which can be translated as  average rated wines. <br>
There are no missing values within the dataset and no categorical columns. <br>
Colinearity between different features can be observed. For machine learning modells, a PCA could be helpfull. <br>
There are some outliers within the values. However, the statistical analysis does not show unrealistic values, so for machine learning, I would prefer to not delete or manipulate them in the first place. <br>
When we look at the different features and their impact on the wine rating, different trends, as well as apparently little effect can be observed(see chapter before). When building a machine learning model, alcohol and volatile acidity will probably have the highest feature importance as the trend can be clearly seen. 
