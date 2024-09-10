
# Causes of Death Analysis Project

## Project Overview

This project focuses on analyzing the causes of death across various countries and categories using statistical tests and machine learning techniques. The dataset contains information such as the cause of death, the number of deaths, and the region/country for multiple years. The primary goal is to gain insights into global health patterns, using both statistical and machine learning approaches to understand trends and variations.

## Features of the Project

- **Data Preprocessing:** The dataset is cleaned, and missing values are handled using methods like imputation.
- **Statistical Tests:**
  - **Shapiro-Wilk Test**: Used to check for the normality of the data.
  - **Kolmogorov-Smirnov Test (KS Test)**: Used for comparing the distribution of death numbers across different causes.
  - **Kruskal-Wallis Test**: Non-parametric test used to compare multiple groups.
- **Clustering**:
  - **K-Means Clustering**: Implemented to categorize countries based on death causes and patterns.
- **Dimensionality Reduction**:
  - **PCA (Principal Component Analysis)**: Used to reduce the complexity of the dataset while maintaining important information.
  
## Requirements

The following Python libraries are used in this project:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`

To install all required dependencies, run:

```bash
pip install -r requirements.txt
```

## Dataset

The dataset includes the following fields:

- **Causes name**: The category of the cause of death (e.g., Meningitis, Neoplasms).
- **Full Description**: A more detailed description of the cause.
- **Death Numbers**: The number of deaths caused by this category in a particular year.
- **Entity (Country)**: The country where the data was collected.
- **Year**: The year the data corresponds to.

## Analysis Approach

1. **Data Preprocessing**: Handling missing values and normalizing data using `MinMaxScaler`.
2. **Statistical Analysis**: Applying statistical tests to verify assumptions and hypotheses about the dataset.
3. **Clustering**: Using K-Means to group countries with similar death patterns.
4. **Dimensionality Reduction**: Applying PCA to visualize and reduce the dataset's complexity while maintaining significant patterns.

## Usage

1. Clone the repository:

```bash
git clone <repository-url>
cd <project-directory>
```

2. Run the Jupyter notebook:

```bash
jupyter notebook
```

3. Follow the cells in the notebook to explore the analysis and results.

## Results and Findings

- The clustering algorithm grouped countries into several clusters based on the most frequent causes of death.
- The KS and Kruskal-Wallis tests showed significant differences between certain causes of death, rejecting the null hypothesis for several categories.

## Conclusion

This project provides a comprehensive analysis of global death causes using both statistical and machine learning approaches. The results could be used to understand trends and aid in public health decisions.