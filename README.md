# EEG Signal Analysis

This repository provides a comprehensive set of tools for analyzing EEG (electroencephalography) signal data. It includes functionality for loading EEG data from a CSV file, computing its Power Spectral Density (PSD), and visualizing the results. The main components of the repository are:

1. **Data Loading**: Methods to read and preprocess EEG signal data from CSV files.
2. **PSD Computation**: Tools for calculating the Power Spectral Density (PSD) of the signal to analyze its frequency components.
3. **Visualization**: Functions to create plots of the time-domain signal and its PSD to aid in understanding the signal's characteristics.

## Features

- **Load EEG Data**: Import EEG signal data from CSV files with time and amplitude columns.
- **Compute PSD**: Use Welch’s method to estimate the Power Spectral Density of the signal.
- **Plotting**: Generate visualizations of both the time-domain signal and its frequency-domain representation.

## Requirements

To run the code in this repository, you need to have the following Python packages installed:

- **`numpy`**: A library for numerical computations and array manipulations.
- **`pandas`**: A library for data manipulation and analysis, especially for handling CSV files.
- **`matplotlib`**: A library for creating static, animated, and interactive visualizations in Python.
- **`scipy`**: A library for scientific and technical computing, including signal processing tools.

You can install these dependencies using pip. Open your terminal or command prompt and run the following command:

```bash
pip install numpy pandas matplotlib scipy
