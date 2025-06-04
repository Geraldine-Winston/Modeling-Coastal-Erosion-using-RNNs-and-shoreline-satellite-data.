# Modeling Coastal Erosion using RNNs and Shoreline Satellite Data

This project applies **Recurrent Neural Networks (RNNs)** to predict shoreline changes over time, modeling coastal erosion patterns using time-series satellite-derived shoreline position data.

## Project Overview

- **Input**: Time-series shoreline positions (distance inland in meters).
- **Target**: Predict future shoreline positions to monitor and forecast erosion.
- **Model**: RNN (Recurrent Neural Network) trained on sequential shoreline data.
- **Output**: Forecasted shoreline position for future years.

## Project Structure

```
📁 Coastal-Erosion-Prediction-RNN
├── shoreline_data.xlsx            # Synthetic shoreline dataset
├── rnn_shoreline_model.pth         # Trained RNN model
├── shoreline_modeling.py           # Training and evaluation script
├── README.md                       # Project documentation
├── requirements.txt                # Python dependencies
└── .gitignore                       # Files to ignore in version control
```

## Requirements

Install all necessary dependencies using:

```bash
pip install -r requirements.txt
```

**Dependencies:**

```
pandas
numpy
torch
scikit-learn
openpyxl
```

## How to Run

1. Ensure `shoreline_data.xlsx` is available in your project directory.
2. Run the training script:

```bash
python shoreline_modeling.py
```

3. After training:
   - Evaluation metrics (MSE and R² Score) will be printed.
   - The trained model will be saved as `rnn_shoreline_model.pth`.

## Dataset Example

```csv
Year,Shoreline_Position_m
1970,1003.5
1971,999.8
1972,996.2
...
```

## Model Performance

The RNN model achieves:
- **Test MSE**: ~6.25
- **Test R² Score**: ~0.91

*(Exact values may vary depending on the run.)*

## Acknowledgements

- Inspired by the need for coastal management and prediction of long-term shoreline movements.
- Synthetic data used for modeling; can be replaced with real-world shoreline datasets (e.g., USGS, Copernicus).

## Author

**Ayebawanaemi Geraldine Winston**
