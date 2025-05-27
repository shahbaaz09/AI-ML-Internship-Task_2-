Task 2: Exploratory Data Analysis (EDA) - AI & ML Internship
This repository contains the solution for Task 2: Exploratory Data Analysis (EDA) as part of the AI & ML Internship by Elevate Labs.

🎯 Objective
The main objective of this task was to understand the dataset using statistical methods and various visualizations. EDA is a crucial step to gain insights, identify patterns, trends, and anomalies before proceeding with machine learning model building.

🛠 Tools Used
 * Python: The primary programming language.
 * Pandas: Essential for data manipulation and generating descriptive statistics.
 * NumPy: Used for numerical operations, supporting Pandas.
 * Matplotlib: A fundamental plotting library for creating static, interactive, and animated visualizations.
 * Seaborn: Built on Matplotlib, providing a high-level interface for drawing attractive and informative statistical graphics.
 * Plotly (Optional): Can be used for interactive visualizations, though Matplotlib and Seaborn were primarily used for this task.
   
📊 Dataset
The Titanic Dataset was used for this task. This dataset was previously cleaned and preprocessed in Task 1, providing a refined basis for performing EDA. The dataset contains information about passengers aboard the Titanic, including their demographics, travel class, and survival status.

📝 Steps Performed
The following steps were undertaken to perform a comprehensive Exploratory Data Analysis on the Titanic dataset:
 * Generate Summary Statistics:
   * Used df.describe() to obtain descriptive statistics (mean, median, standard deviation, min, max, quartiles) for numerical features.
   * Analyzed value_counts() for categorical features (after encoding) to understand their distribution and frequency.
   * Inference: This initial statistical overview provided insights into the central tendency, spread, and range of the data, highlighting potential skewness or extreme values.
 * Create Histograms and Boxplots for Numeric Features:
   * Histograms: Generated histograms for numerical columns (e.g., 'Age', 'Fare', 'SibSp', 'Parch') to visualize their distributions, identify skewness, and observe data density. kde=True was used to overlay a kernel density estimate.
   * Boxplots: Created boxplots for the same numerical features to visualize their quartiles, median, and to easily identify outliers and the spread of data.
   * Inference: Visual inspection of these plots confirmed distributions (e.g., normal, skewed), the presence of outliers, and the range of values for each feature.
 * Use Pairplot / Correlation Matrix for Feature Relationships:
   * Correlation Matrix: Calculated and visualized the correlation matrix using a heatmap (sns.heatmap). This helped in understanding the linear relationships between all pairs of numerical features. High correlation between independent variables might indicate multicollinearity.
   * Pairplot: Utilized sns.pairplot() to visualize relationships between selected pairs of features (e.g., 'Survived', 'Age', 'Fare', 'Pclass') along with their individual distributions. The hue='Survived' parameter was particularly useful for observing how feature relationships varied with survival status.
   * Inference: This step was crucial for identifying potential multicollinearity and understanding which features had a strong linear relationship with each other or with the target variable ('Survived').
 * Identify Patterns, Trends, or Anomalies:
   * Created various plots to explore relationships between features and the target variable ('Survived').
   * Categorical vs. Numerical: For example, sns.histplot(x='Age', hue='Survived') was used to analyze age distribution across survivors and non-survivors.
   * Categorical vs. Categorical: sns.countplot(x='Pclass', hue='Survived') was used to examine survival rates across different passenger classes.
   * Inference: Discovered insights such as potential age groups with higher survival rates, the impact of passenger class on survival, and other interesting demographic patterns.
 * Make Basic Feature-Level Inferences from Visuals:
   * Summarized observations drawn from the visualizations and statistical analyses.
   * Identified which features appeared to be strong predictors of survival (e.g., 'Pclass', 'Sex', 'Age' to some extent).
   * Noted any features exhibiting significant skewness or a high number of outliers, which were handled in Task 1.
   * Discussed any unexpected trends or insights that emerged from the data exploration.
     
🧠 What Was Learned
This task significantly enhanced understanding in:
 * Data Visualization: Proficiency in using Matplotlib and Seaborn to create various types of plots for data exploration.
 * Descriptive Statistics: Ability to generate and interpret summary statistics to understand data distributions.
 * Pattern Recognition: Skill in identifying trends, relationships, and anomalies within the dataset through visual and statistical analysis.
 * Role of EDA: Reinforced the understanding that EDA is a critical preliminary step in any ML project, providing the necessary groundwork for informed model building.
📁 Repository Contents
 * titanic_cleaned.csv: The cleaned and preprocessed dataset from Task 1, used as the basis for EDA.
 * [task_2].ipynb: The Jupyter Notebook containing all the Python code for performing EDA, including statistical summaries and visualizations.
