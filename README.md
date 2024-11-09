
# Synthetic Data Generation for UCI Mechanical Analysis Dataset

## Description
This project generates synthetic data to extend the [UCI Mechanical Analysis Data Set](https://www.kaggle.com/datasets/heitornunes/mechanical-analysis) by interpolating intermediate points between existing data points. The goal is to create a larger dataset while maintaining the statistical relationships present in the original data, which is useful for tasks that benefit from an expanded dataset, such as machine learning model training and statistical analysis.

## Table of Contents
- [Background](#background)
- [Dataset](#dataset)
- [Features](#features)
- [Data Generation Process](#data-generation-process)
- [Correlation Analysis](#correlation-analysis)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [License](#license)

## Background
In data science, having a large and representative dataset can significantly improve the performance of machine learning models. This project extends the UCI Mechanical Analysis Dataset by generating additional synthetic data points through interpolation. A key part of this process is to validate that the extended dataset maintains the statistical properties of the original dataset.

## Dataset
The original dataset used in this project is the **UCI Mechanical Analysis Data Set**. This dataset contains various mechanical attributes, which are extended with synthetic data to increase the dataset size and improve its utility in analysis and machine learning applications. You can find more information about this dataset on the [UCI Machine Learning Repository](https://www.kaggle.com/datasets/heitornunes/mechanical-analysis).

## Features
- Generates synthetic data points through interpolation between existing data points.
- Extends the UCI Mechanical Analysis Dataset while maintaining the original correlation structure.
- Validates the synthetic data by comparing correlation matrices of the original and extended datasets.
- Provides correlation matrix visualizations to ensure consistency in data patterns.

## Data Generation Process
1. **Data Scaling and Imputation**: Preprocesses the original data by scaling and imputing missing values to ensure that all features are in comparable ranges.
2. **Synthetic Data Generation**: Interpolates intermediate data points between original data points to create synthetic data.
3. **Combining Datasets**: Combines the original dataset with the generated synthetic data to form a larger dataset.
4. **Validation**: Performs correlation analysis to verify that the synthetic data aligns with the patterns of the original data.

## Correlation Analysis
To ensure that the extended dataset retains the statistical characteristics of the original dataset, correlation matrices are calculated for both datasets. These matrices are visualized to check if feature relationships are consistent between the original and extended datasets.

## Installation
1. Clone the repository:
   ```bash
   git clone <https://github.com/RadmehrA/Synthetic-Data-Generation_UCI-Mechanical-Analysis-Data-Set.git>
   cd <https://github.com/RadmehrA/Synthetic-Data-Generation_UCI-Mechanical-Analysis-Data-Set/>
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. **Prepare Data**: Place your UCI Mechanical Analysis dataset in the designated directory or load it in the script as instructed.
2. **Run the Data Generation Script**:
   ```bash
   python data_generation.py
   ```
3. **Run Correlation Analysis**: Execute the correlation analysis script to visualize and compare the correlation matrices of the original and extended datasets.

## Project Structure
- `data/`: Directory containing the UCI Mechanical Analysis dataset.
- `output/`: Directory where the extended dataset and correlation analysis plots are saved.
- `data_generation.py`: Script for generating synthetic data.
- `correlation_analysis.py`: Script for performing correlation analysis and plotting correlation matrices.
- `requirements.txt`: Python dependencies.

## Dependencies
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn

Install dependencies with:
```bash
pip install -r requirements.txt
```

## License
This project is licensed under the MIT License.
