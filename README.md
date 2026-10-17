# Smart City Traffic Flow Simulator

A Python project built with **NumPy** in Google Colab to simulate hourly vehicle traffic at 10 city junctions over 30 days and identify peak congestion periods.

## Project Objective

Simulate vehicle counts for 30 days across 10 junctions, model morning and evening rush-hour patterns, and analyze the results to find traffic bottlenecks.

## Technologies Used

- Python
- NumPy
- Matplotlib (for visualizations, if used)
- Google Colab

## Features

- Simulates traffic using NumPy's Poisson random distribution.
- Models hourly traffic counts for 30 days and 10 junctions.
- Includes higher traffic during morning and evening rush hours.
- Aggregates traffic counts by day, junction, and hour.
- Identifies peak traffic hours using `argmax()`.
- Visualizes traffic patterns with a heatmap.
- Compares loop-based calculations with vectorized NumPy operations.
- Uses a reproducible random seed for consistent results.

## Simulation Details

- **Days:** 30
- **Junctions:** 10
- **Hours per day:** 24
- **Total junction-hour records:** 30 × 10 × 24 = 7,200
- **Traffic model:** Poisson distribution

## How It Works

1. Import NumPy and set a random seed.
2. Create an hourly traffic curve with morning and evening rush-hour peaks.
3. Generate simulated vehicle counts using `np.random.poisson()`.
4. Aggregate traffic data along the required axes.
5. Find peak traffic hours and busiest junctions using `np.argmax()`.
6. Plot a heatmap to visualize traffic intensity.
7. Compare loop-based and vectorized calculations using `%timeit`.

## How to Run

### Google Colab

1. Open Google Colab.
2. Upload or open the notebook file.
3. Run each code cell from top to bottom.
4. Review the summary statistics and generated visualizations.

### Local Python Setup

1. Install Python.
2. Install the required libraries:

   ```bash
   pip install numpy matplotlib
   ```

3. Run the notebook in Jupyter Notebook or JupyterLab.

## Project Structure

```text
Smart-City-Traffic-Flow-Simulator/
├── Smart_City_Traffic_Flow_Simulator.ipynb
└── README.md
```

## Learning Outcomes

This project demonstrates:

- NumPy array creation and multidimensional shapes
- Random number generation with `np.random.poisson()`
- Axis-wise aggregation
- Finding maximum values and their indices with `argmax()`
- Heatmap visualization
- Vectorized operations versus loops
- Basic traffic data analysis

## Resume Description

Built a reproducible NumPy-based traffic simulator in Google Colab to generate 7,200 junction-hour records using a Poisson model; identified peak congestion windows with axis-wise aggregation and `argmax()`, and compared vectorized and loop-based code.

## Author

Chahit Chhajlani
