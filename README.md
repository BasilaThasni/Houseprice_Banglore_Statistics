#House Price in Banglore-Data analysis:
# Bangalore Property Price Analysis

This project analyzes property prices in Bangalore to understand the distribution, detect and handle outliers, and examine relationships between variables. The analysis is based on the `house_price.csv` dataset, which includes information about property prices per square foot, among other features.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Objective](#objective)
- [Methodology](#methodology)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The goal of this project is to perform exploratory data analysis (EDA) on property prices in Bangalore, detect and treat outliers, and visualize data to better understand price distribution and relationships between key variables.

## Dataset

The dataset `house_price.csv` contains information about properties in Bangalore, including the following columns:
- **price_per_sqft**: Property price per square foot
- **location**: Location of the property
- **size**: Size of the property (e.g., 2 BHK, 3 BHK)
- **area_type**: Type of area (e.g., Super Built-Up Area, Plot Area)
  
### Assumptions
Additional assumptions may be needed if the column descriptions are not provided in the dataset. These can be adjusted based on further analysis or domain knowledge.

## Objective

1. **Exploratory Data Analysis (EDA)**: Understand the data structure, distribution, and basic statistics.
2. **Outlier Detection and Treatment**: Identify and handle outliers using multiple statistical methods:
   - Mean and Standard Deviation
   - Percentile Method
   - Interquartile Range (IQR) Method
   - Z-Score Method
3. **Data Transformation**: Apply transformations if necessary to normalize data distribution.
4. **Correlation and Visualization**: Examine relationships between numerical variables using heatmaps, scatter plots, and other visual tools.

## Methodology

### Step 1: Basic EDA
- Analyze the data types, summary statistics, and missing values.
- Check for unique values in categorical columns and inspect the distribution of numerical features.

### Step 2: Outlier Detection and Removal
- Detect and remove outliers using multiple statistical methods and determine which method is most effective by visual inspection of box plots.

### Step 3: Data Transformation
- Analyze the distribution of `price_per_sqft` using histograms, skewness, and kurtosis. Apply transformations to normalize if necessary.

### Step 4: Correlation and Visualization
- Use heatmaps and scatter plots to identify relationships between key variables and analyze the data structure.

### Step 5: Visualization
- Plot histograms, box plots, and scatter plots to present the distribution, outliers, and correlations within the data.

## Results

- **Outlier Removal**: Comparison of outlier detection methods and their effectiveness in cleaning data.
- **Data Normalization**: Evaluation of skewness and kurtosis before and after transformations.
- **Correlation Analysis**: Identification of relationships between numerical features in the dataset.

  ## Inferences and Insights

1. **Price Distribution**: Property prices per square foot in Bangalore have a right-skewed distribution, with a few extremely high-value properties affecting the overall mean. Applying transformations such as log scaling effectively normalized this distribution.
   
2. **Outlier Detection**: The Interquartile Range (IQR) method proved the most effective in balancing outlier removal while retaining most data points. It provided a clear representation of data distribution without excessive trimming.

3. **Correlation**: Significant correlations were observed between certain property attributes (e.g., `size` and `price_per_sqft`), which suggests that property size may play an influential role in pricing. However, further feature engineering might be required to understand more complex relationships.

4. **Location Impact**: Location variations led to substantial price differences, emphasizing that property prices in Bangalore are highly location-sensitive. This may imply the need for clustering techniques to segment data for finer-grained insights.

## Technologies Used

- **Python**: Programming language used for analysis
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib & Seaborn**: Data visualization libraries
- **SciPy**: Used for Z-score calculations and transformations

