# Power Spectral Density (PSD) Analysis

This repository contains tools for analyzing Power Spectral Density (PSD) of EEG signals. It includes functionality to load EEG data, compute PSD using Welch's method, and visualize the results. Below is a brief explanation of the theory behind PSD and Welch's method.

## Theory

### Power Spectral Density (PSD)

**Power Spectral Density (PSD)** is a fundamental concept in signal processing that represents how power (or variance) of a signal is distributed with respect to frequency. For EEG signals, PSD is crucial for understanding the distribution of brain activity across different frequency bands. This helps in:

- **Detecting Brain Activity Patterns**: Identifying cognitive and emotional states by analyzing frequency components.
- **Diagnosing and Monitoring Neurological Conditions**: Evaluating abnormalities and tracking the progression of conditions.
- **Developing Biomarkers**: Creating indicators for clinical and research studies.
- **Filtering Signals**: Removing noise and artifacts to get a clearer representation of the EEG signal.
- **Understanding Brain-Behavior Relationships**: Linking cognitive and emotional states with brain activity.

### Welch's Method

**Welch's Method** is a technique used to estimate the Power Spectral Density (PSD) of a signal, offering improvements over the basic periodogram method. It reduces variance and provides a more accurate PSD estimate by:

1. **Segmenting the Signal**: Dividing the signal into overlapping segments. This ensures that the entire signal is used for the estimation, improving accuracy.
2. **Applying Window Functions**: Multiplying each segment by a window function (such as Hamming, Hanning, or Blackman) to reduce edge effects and spectral leakage. This minimizes discontinuities at segment boundaries, leading to a more precise PSD estimate.
3. **Calculating Periodograms**: For each windowed segment, computing the periodogram, which is the squared magnitude of the Fourier Transform. The periodogram provides an estimate of the PSD for that segment.
4. **Averaging Periodograms**: Averaging the periodograms of all segments to produce the final PSD estimate. This averaging process reduces variance compared to using a single periodogram, resulting in a smoother and more reliable PSD.
5. **Normalization**: Adjusting the final PSD estimate to account for overlapping and window effects, ensuring that the PSD values are correctly scaled.

## Requirements

To run the code in this repository, you need to have the following Python packages installed:

- **`numpy`**: A library for numerical computations and array manipulations.
- **`pandas`**: A library for data manipulation and analysis, especially for handling CSV files.
- **`matplotlib`**: A library for creating static, animated, and interactive visualizations in Python.
- **`scipy`**: A library for scientific and technical computing, including signal processing tools.

You can install these dependencies using pip. Open your terminal or command prompt and run the following command:

```bash
pip install numpy pandas matplotlib scipy
