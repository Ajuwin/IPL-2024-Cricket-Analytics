# IPL-2024-Cricket-Analytics

## Overview

This project analyzes IPL 2024 match data using PySpark, focusing on player and team performances. The data is stored in Hadoop and processed with Apache Spark to derive meaningful insights.

## Tech Stack

- **PySpark**: Data processing and transformations
- **Hadoop**: File storage and retrieval (Optional)
- **Jupyter Notebook**: Interactive data analysis

## Data Sources

The dataset includes:

- **Ball-by-ball data**: Every delivery's details (runs, wickets, extras, etc.)
- **Match metadata**: Team details, match results, umpires, and venues

## Key Analyses

- Highest individual scores and partnerships
- Best bowling performances in powerplay and death overs
- Toss impact on match outcomes
- Successful run chases in the last over
- Team with the best powerplay average score

## Project Structure

```
IPL-2024-Data-Engineering/
│── data/                    # Raw dataset (CSV)
    |── ball_by_ball.csv
    |── matches.csv
│── IPL_2024_Analysis.ipynb  # Main Jupyter Notebook
│── README.md                # Project documentation
```

## Running the Project

### Prerequisites

- Hadoop installed and configured (Optional)
- Spark installed
- Jupyter Notebook setup

### Steps to Run

1. Start Hadoop services (if using Hadoop): `start-dfs.sh && start-yarn.sh`
2. Load data into Hadoop (if applicable): `hdfs dfs -put local_file_path /hadoop_directory`
   If Hadoop is not used, update the file path in the scripts to read from the local file system instead.
3. Run Jupyter Notebook: `jupyter notebook`
4. Execute analysis notebooks to generate insights
