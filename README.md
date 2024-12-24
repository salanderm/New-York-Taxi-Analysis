# Taxi Data Analysis

## Overview
This project analyzes taxi trip data from January 2024 to identify trends, patterns, and insights about passenger behavior, trip details, and revenue metrics. The dataset provides information such as pickup and dropoff times, trip distances, payment types, and fares.

## Features
- **Data Loading**: Load and concatenate taxi data from CSV files.
- **Data Cleaning**: Handle mixed data types, convert columns to appropriate formats, and remove unnecessary features.
- **Exploratory Analysis**:
  - Temporal patterns (e.g., busiest hours of the day).
  - Spatial trends (e.g., most frequent pickup and dropoff locations).
  - Revenue analysis (e.g., average fare by distance).
- **Visualization**: Use charts to represent patterns in trip frequency, distance, and payment types.

## Dataset
- **Source**: Yellow Taxi Trip Data (January 2024).
- **Size**: 2,964,624 rows and 19 columns.
- **Key Columns**:
  - `tpep_pickup_datetime`, `tpep_dropoff_datetime`: Start and end times of trips.
  - `trip_distance`: Distance of each trip in miles.
  - `PULocationID`, `DOLocationID`: Pickup and dropoff location IDs.
  - `payment_type`: Type of payment used (e.g., cash, card).
  - `total_amount`: Total fare for the trip.

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/taxi-data-analysis.git
   cd taxi-data-analysis
   ```
2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Place the taxi data CSV file in the `data/` directory.
2. Run the notebook:
   ```bash
   jupyter notebook taxi_analysis.ipynb
   ```
3. Explore the analysis and visualize results.

## File Structure
```
project-root/
|-- data/                # Folder containing raw data files
|-- taxi_analysis.ipynb  # Jupyter notebook with analysis steps
|-- requirements.txt     # Python dependencies
|-- README.md            # Project documentation
```

## Results
### Key Insights
- **Busiest Hours**: Peak trip activity occurs during evening rush hours.
- **Popular Locations**: Location IDs 79 and 186 are the most frequent pickup spots.
- **Revenue Trends**: Trips with longer distances tend to yield higher fares, but there are diminishing returns beyond a certain point.

## Future Work
- Integrate weather and holiday data for richer context.
- Develop predictive models to forecast trip counts and fare revenue.
- Build an interactive dashboard for real-time insights.

## Contributing
Contributions are welcome! Please submit a pull request or create an issue to propose changes or new features.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
Special thanks to the NYC Taxi & Limousine Commission for providing the data used in this analysis.
