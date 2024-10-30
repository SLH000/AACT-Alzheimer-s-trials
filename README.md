# Alzheimer's Disease Clinical Trial Dashboard

## Overview

The Alzheimer's Disease Clinical Trial Dashboard is an interactive Streamlit tool that provides insights into ongoing and completed clinical trials for Alzheimer's Disease (AD) and Mild Cognitive Impairment (MCI). It allows users to filter by year range and trial phase, view trial distribution over time, explore sponsor data, and visualize trends in research focus.

## Features

- **Data Filtering:** Filter trials by year range and phase.
- **Real-Time Auto-Refresh:** Enable optional auto-refresh to update data in real-time.
- **Visualizations:** Explore trends through line charts, bar charts, and pie charts.
- **Sponsor and Condition Analysis:** Visualize the distribution of trials by sponsor and specific conditions.

## Installation

1. **Clone the Repository**:
```bash
git clone https://github.com/yourusername/ad-clinical-trial-dashboard.git
cd ad-clinical-trial-dashboard
``` 

2. **Install the required packages:**
```bash

pip install streamlit pandas psycopg2 matplotlib seaborn plotly streamlit-autorefresh
Usage
```

3. **Database Configuration: Update the database connection with your credentials in the script:**
```python
conn = psycopg2.connect(
    host="aact-db.ctti-clinicaltrials.org",
    port="5432",
    user="your_username",
    password="your_password",
    database="aact"
)
```
4. **Run the Dashboard**
Start the Streamlit application:
```bash
streamlit run app.py
```

## Dashboard Overview
Access the following functionalities in the dashboard:
- Date Range and Phase Selection: Filter trials by year and phase.
- Visualizations:
    - Line chart showing trials over time.
    - Pie chart for phase distribution.
    - Bar charts for sponsor vs. phase and trial counts by condition.

## Dashboard Layout

1. Title and Description: Provides an overview of the dashboard's purpose.
2. Controls:
    - Year Range Selector: Filter trials by start and completion year.
    - Phase Selector: Choose specific phases of interest.
3. Visualizations:
    - Trials Over Time: Line chart for the number of new trials each year.
- Trial Phase Distribution: Pie chart visualizing the breakdown of trial phases.
- Sponsor and Condition Distribution: Bar charts showing sponsor vs. phase and conditions distribution.

## Footer: 
Links to ClinicalTrials.gov as the data source.
## Data Source

Data is sourced from the publicly accessible AACT database hosted by ClinicalTrials.gov.

## License

This project is licensed under the MIT License.

