PySpark Data Engineering Scenarios
Project Overview
This repository contains PySpark-based data engineering solutions developed using real-world, multi-domain product and review datasets. These projects simulate common data engineering scenarios such as ETL, data aggregation, analytics, and recommendation system feature engineering—all solvable with PySpark and Spark SQL, and designed for easy local execution.

Datasets Used
The following datasets are included:

All-Appliances.csv

All-Books.csv

All-Electronics.csv

All-Exercise-and-Fitness.csv

All-Home-and-Kitchen.csv

All-Sports-Fitness-and-Outdoors.csv

amazon_reviews.csv

Baby-Products.csv

Camera-Accessories.csv

Car-Accessories.csv

Diet-and-Nutrition.csv

Home-Dcor.csv

Kindle-eBooks.csv
Each file contains structured data on products or user reviews across categories.

Scenario Questions
Solutions are provided for scenarios of varying complexity. Each scenario is designed to be a standalone project and includes documented PySpark or Spark SQL code.

Easy
Product Ratings Aggregation: Find average rating for each product sub-category and list top products.

Review Statistics: Calculate total reviews and average user scores by app version.

Medium
Multi-Category Analytics: Join multiple product datasets and analyze top products by ratings and discounts.

Ratings vs Review Scores: Correlate product ratings with review scores for consistency checks.

Hard
Recommendation Feature Prep: Generate user-product interaction matrices for recommender systems.

Discount Trends Over Time: Analyze historical pricing to detect trends and seasonality.

Solution Approach
Ingest CSV files using PySpark

Perform ETL operations like data cleaning, type casting, aggregation, and joining

Use Spark SQL for complex querying and analytical calculations

Output results to clean CSV/JSON/parquet files for analysis or reporting

All code is modular, documented, and reusable

How to Run
Requirements

Python 3.7+

PySpark

pandas (optional for local inspection)

Jupyter Notebook or PyCharm IDE

Setup

bash
pip install pyspark pandas
Download all CSV datasets to a local data/ directory.

Execution

Run individual scenario scripts/modules from the project.

Example:

bash
spark-submit scenarios/easy_product_ratings.py
Results

Output files are stored in the output/ folder.

Script logs provide execution details and summary statistics.

Repository Structure
text
data/
  └── [CSV DATASETS]
scenarios/
  ├── easy_product_ratings.py
  ├── medium_multi_category_analytics.py
  ├── hard_recommender_feature_prep.py
output/
  └── [RESULTS]
README.md
requirements.txt
Contributing
Feel free to open issues or PRs for improvements, additional scenario ideas, or enhancements to existing modules.

License
This project is released under the MIT License.

