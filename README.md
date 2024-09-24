# Electric Vehicle Charging Station Management

## Overview

This project is designed to manage electric vehicle (EV) charging sessions, track energy consumption, and predict the cost of future charging sessions using machine learning. The system includes a Python class to manage charging sessions, a dataset management system using DVC, and an AutoML pipeline for cost prediction.

## Project Structure

- **ChargingStationManager.py**: Contains the `ChargingStationManager` class for tracking charging sessions.
- **data/**: Directory to store datasets, including `ev_charging.csv`.
- **models/**: Directory for storing trained machine learning models.
- **notebooks/**: Jupyter notebooks for exploratory data analysis and model training.
- **requirements.txt**: Python package dependencies.
- **dvc.yaml**: DVC pipeline configuration.
- **.gitignore**: Files to ignore in the Git repository.

## Features

1. **Charging Session Management**:
   - A Python class `ChargingStationManager` to track and manage EV charging sessions.
   - Methods to add new charging sessions and compute total energy consumption for each vehicle.

2. **Data Version Control (DVC)**:
   - Utilizes DVC to manage the dataset (`ev_charging.csv`) for tracking vehicle charging sessions.
   - Ability to modify the dataset and commit changes with DVC commands.

3. **AutoML Pipeline**:
   - Implements an AutoML pipeline to predict the energy cost of future charging sessions.
   - Trains multiple models including `LinearRegression`, `RandomForestRegressor`, and `SVR`, and selects the best-performing model based on validation metrics.

4. **Version Control with Git**:
   - Set up a Git repository with a branching structure:
     - **main**: Stable production code.
     - **development**: Development of new features.
     - **feature/**: Individual feature branches for specific enhancements.
   - Merging strategies to ensure the `main` branch is updated with stable code after thorough testing.

