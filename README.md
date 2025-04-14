# Zuber Ride-Share Analysis – Chicago, November 2017

This project analyzes Chicago taxi ride data to support the market entry strategy of **Zuber**, a new ride-sharing company. The analysis explores passenger ride patterns, company performance, popular drop-off locations, and the impact of weather on trip duration.

## Project Structure

This project is implemented in a Jupyter Notebook: **`Ride Share Analysis.ipynb`**

### Key Objectives:
- Analyze trip data and weather records to identify patterns.
- Compare ride frequency across taxi companies and neighborhoods.
- Visualize top-performing companies and locations.
- Test the hypothesis: *"The average ride duration from the Loop to O'Hare changes on rainy Saturdays."*

## Tools and Technologies

- **Python (Pandas, Matplotlib, Seaborn, SciPy)**
- **SQL** (data retrieval and aggregation)
- **Jupyter Notebook**
- **HTML parsing** (for weather data)
- **Statistical testing** (two-sample t-test)

## Data Sources

1. SQL database containing:
   - `neighborhoods`: Neighborhood metadata
   - `cabs`: Taxi company and vehicle information
   - `trips`: Ride-level detail
   - `weather_records`: Hourly weather data

2. CSV files used for further analysis:
   - `project_sql_result_01.csv`: Taxi company ride counts (Nov 15–16, 2017)
   - `project_sql_result_04.csv`: Avg drop-offs per neighborhood
   - `project_sql_result_07.csv`: Ride durations and weather conditions

3. HTML page (web-scraped):
   - Weather records from November 2017

## Hypothesis Tested

> **"Ride durations from the Loop to O’Hare differ on rainy Saturdays."**

- Null Hypothesis (H₀): There is no difference in mean ride durations.
- Alternative Hypothesis (H₁): Ride durations differ when it’s raining.
- Significance Level: α = 0.05
- Method: Two-sample t-test

## Key Insights

- Flash Cab and Taxi Affiliation Services were the top ride providers mid-month.
- Drop-offs were most frequent in central neighborhoods like The Loop.
- A statistically significant difference in ride duration was observed during rainy conditions, suggesting weather may affect trip times.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/zuber-ride-analysis.git
   cd zuber-ride-analysis

2. Open the Jupyter Notebook:
    jupyter notebook "Ride Share Analysis.ipynb"

3. Run the notebook cells to follow the full analysis pipeline.
