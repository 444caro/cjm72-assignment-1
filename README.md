# Elevator Optimal Waiting Position
This project was completed for **Assignment 1: Data Collection and Analysis** in CS506: Computing and Data Science at Boston University. The goal was to determine the best location to wait for an elevator in the CDS building lobby, minimizing expected walking distance based on collected arrival data.

## Objective
Using a shared dataset of elevator arrival times collected by the class, we analyzed elevator usage patterns and used statistical and spatial reasoning to compute the optimal place to wait for an elevator.

## Learning Goals
- Practice collecting and visualizing real-world data.
- Formulate and test hypotheses based on training and evaluation data.
- Apply statistical analysis and spatial modeling.

## Methods
- **Data Collection**: Timestamped elevator IDs were recorded during 5-minute observation slots across 4 days.
- **Visualization**: Arrival data was plotted using `matplotlib` and `seaborn` to identify usage patterns.
- **Statistical Analysis**: Frequency of elevator arrivals was calculated and normalized into a probability distribution.
- **Optimization**: The best standing location was computed using a weighted average of elevator coordinates.
- **Evaluation**: Average walking distances were computed using both training and test datasets to validate the hypothesis.

## 📈 Results
| Location | Training Avg. Distance (m) | Test Avg. Distance (m) |
|----------|-----------------------------|--------------------------|
| Naive guess (3,2) | 2.1882 | 2.1882 |
| Optimal guess (3.06, 1.47) | 2.1674 | 2.1674 |
