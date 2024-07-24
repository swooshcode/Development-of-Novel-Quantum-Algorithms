# Quantum Portfolio Optimization

## Overview
This project leverages quantum computing to optimize financial portfolios using real-world data.

## Methodology
1. **Data Collection:** 
   - Historical data for S&P 500, EuroStoxx 50, Nikkei 225, FTSE 100, and Gold was fetched using the Yahoo Finance API.
   - The data range is from January 2019 to May 2024.

2. **Data Preprocessing:**
   - Filled missing values using forward fill.
   - Calculated daily returns.

3. **Model Creation:**
   - Created a Binary Quadratic Model (BQM) using mean returns and correlation matrix.

4. **Optimization:**
   - Used the D-Wave Leap Hybrid Sampler to solve the BQM and find the optimal portfolio.

## Results
- **Optimal Portfolio:** Selected assets corresponding to indices 2 (Nikkei 225).
- **Quantum Computation Time:** Approximately 3.54 seconds.

## Further Development: Scalability Testing

### Methodology
- Define a larger Binary Quadratic Model (BQM) for different problem sizes.
- Measure the quantum computation time for each problem size.

### Results
- Computation times for problem sizes: [10, 20, 30, 40, 50]
- Quantum Times: [3.99, 3.60, 3.47, 3.67, 3.73] seconds

## Files
- `src/`: Source code for data processing and optimization.
- `notebooks/`: Jupyter notebooks for interactive analysis.
- `docs/`: Detailed documentation.
- `presentation/`: Presentation summarizing the project.

## Setup
1. Install requirements: `pip install -r requirements.txt`
2. Run the data fetching: `python src/fetch_data.py`
3. Run the data preprocessing: `python src/preprocess_data.py`
4. Run the optimization: `python src/solve_bqm.py`
5. Measure computation time: `python src/measure_time.py`

## Authors
- Nigel K. Phillips 
