# ⚡ Energy Demand Prediction & Peak Load Analysis

## Project Overview
This project addresses the concern of an energy company (eSC) regarding the impact of global warming on electricity demand. The primary goal is to predict and manage potential peak energy usage, particularly during a "hotter-than-normal" summer, to prevent blackouts and avoid the need to build a new power plant. The analysis focuses on energy usage in July, which is typically the month with the highest demand.

## Data Sources
The project utilizes several large-scale datasets from Amazon AWS S3, including:
* **Static House Data**: Basic information for approximately 5,000 single-family houses, including house size and building ID.
* **Energy Usage Data**: Hour-by-hour energy usage for each of the 5,000 houses.
* **Metadata**: A human-readable file describing the attributes in the house and energy data files.
* **Weather Data**: Hour-by-hour weather information for approximately 50 geographic counties in South and North Carolina.

## Technical Approach
This project follows a data-driven approach to predict and analyze energy demand.

### Data Preparation
* The first step is to read and merge the provided data from various sources.
* The data is large-scale, with files in 'parquet' and 'CSV' formats.

### Modeling & Analysis
* **Exploratory Data Analysis**: Conduct basic analysis to gain initial insights from the data.
* **Predictive Modeling**: Build and evaluate several regression models to predict hourly energy usage for July.
* **Future Demand Evaluation**: Use the best-performing model to predict future peak energy demand by simulating a scenario where all July temperatures are 5 degrees warmer.
* **Peak Demand Analysis**: Show future peak energy demand for different geographic regions and other important attributes.
