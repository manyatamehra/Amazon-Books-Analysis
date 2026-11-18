# Amazon Books Data Analysis

## Project Overview
An exploratory data analysis project using an Amazon books dataset containing over 33,000 records. The project focuses on understanding book prices, publication trends, available formats, credited names, and data quality.

## Objectives
- Explore and understand the dataset.
- Clean inconsistent and missing data.
- Analyse book prices and publication trends.
- Examine book formats and credited names.
- Identify data-quality issues.
- Create visualisations and export summary reports.

## Dataset
- Total records: 33,505
- Unique book titles: 25,540
- Original columns: Book Name, Book Price, Book Author, Book Rating, Book Release Date, Book Image.

The dataset does not contain a category column, so category-based analysis was not performed.

## Tools & Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- VS Code

## Key Findings
- Average book price: ₹645.07
- Median book price: ₹288
- Zero-price records: 8,666 (25.86%)
- Unique credited names: 8,132
- Suspicious publication dates flagged: 491

The difference between the average and median price suggests that higher-priced listings influence the average.

## Data Cleaning
- Cleaned price values by removing commas and trailing decimal points.
- Converted price and rating columns into numeric formats.
- Separated book formats mistakenly stored in the author column.
- Converted publication dates into datetime format.
- Extracted publication years.
- Flagged suspicious publication dates.
- Investigated missing values and repeated book titles.

## Visualisations
The project includes visualisations exploring:
- Book price distributions.
- Price ranges.
- Average and median prices by format.
- Publication trends by year and month.
- Book format distribution.
- Top credited names.
- Rating-value distribution.

## Reports
Summary reports are available in the `reports/` folder, including descriptive statistics, missing-value summaries, price ranges, format counts, correlation analysis, and key findings.

## Data Limitations
- Zero-price records may represent missing or unreliable price information.
- The meaning of the `Book_Rating` column has not been independently verified.
- Author information contains missing values and publisher/editorial-board names.
- Repeated titles may represent different editions or listings.
- Some metadata may be inaccurate or mismatched.

## Project Structure

Amazon_Books_Analysis/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   └── 01_data_exploration.ipynb
│
├── visualizations/
├── reports/
└── README.md
```

## Conclusion
This project demonstrates an end-to-end exploratory data analysis workflow, from data cleaning and validation to statistical analysis, visualisation, and reporting.

Project Status: Completed
