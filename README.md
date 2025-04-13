# Advanced Ad Pricing Platform for a Society and Township Management Platform

## Overview

The **Advanced Ad Pricing Platform** is a powerful tool designed for society and township management systems to dynamically adjust and optimize ad pricing across various locations and campaign types. This platform uses machine learning to simulate and predict cost-per-click (CPC) prices based on multiple factors, creating insights into ad performance and campaign effectiveness.

## Key Features

- **Real-Time Ad Pricing Simulation**:
  - Continuously generates synthetic ad data to simulate different campaign types across cities, seasons, income levels, and other metrics.

- **Machine Learning-Driven Predictions**:
  - **Global Ad Pricing Model**: Utilizes a Random Forest Regressor to analyze and predict CPC across all locations.
  - **Location-Specific Models**: Tailored models for individual locations to capture city-specific ad performance and pricing dynamics.

- **Database Management and Data Buffering**:
  - Efficient data storage with SQLite.
  - Advanced buffer for managing real-time data influx.

- **Advanced Data Preprocessing**:
  - Feature engineering and encoding for variables such as location, season, and campaign type.
  - Scaler and label encoders to improve prediction accuracy.

- **Interactive Ad Pricing Dashboard**:
  - **Bar Chart**: Displays average CPC by location.
  - **Box Plot**: Shows CPC distribution, helping identify pricing outliers.
  - **Pie Chart**: Highlights the distribution of different campaign types.
  - **Scatter Plot**: Tracks CPC trends over time for ongoing analysis.

## How It Works

1. **Data Generation and Storage**:
   - Synthetic ad data is generated and stored in a structured SQLite database.

2. **Data Loading and Preprocessing**:
   - Data is periodically loaded, cleaned, and encoded to create robust feature sets for model training.

3. **Model Training**:
   - **Global Model**: Trains on all locations and campaigns to establish a baseline CPC prediction.
   - **Location-Specific Models**: Models for each location that meet the minimum data requirement are trained for enhanced locality-specific insights.

4. **Dashboard Creation**:
   - An interactive dashboard provides users with a visual understanding of pricing trends, campaign performance, and CPC variance.

5. **Simulation Execution**:
   - The platform runs a continuous simulation, periodically generating new data, updating models, and refreshing the dashboard with the latest predictions and insights.

This platform combines robust machine learning with visual insights, enabling township and society managers to better understand ad pricing trends and optimize for campaign success.

## Installation

To install the necessary dependencies, open a terminal or command prompt, navigate to your project directory, and run:

```bash
pip install -r requirements.txt
