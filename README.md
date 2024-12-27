# Model Identification for Time-Independent Non-Newtonian Fluids

This project performs model fitting for experimental stress-strain data to identify the best-fit rheological model for time-independent non-Newtonian fluids. The user can input custom stress and strain data, and the program evaluates three models:

1. **Power-Law Model**
2. **Bingham Plastic Model**
3. **Herschel-Bulkley Model**

The project computes the best-fit parameters and evaluates the models using the coefficient of determination ( R²). A visualization of the model fits is also provided.

## Features
- Allows user input for stress and strain data.
- Fits data to three rheological models using nonlinear regression.
- Calculates R² values for model evaluation.
- Automatically identifies the best-fit model.
- Generates a plot comparing experimental data with model predictions.

## Requirements

- Python 3.7 or higher
- NumPy
- Matplotlib
- SciPy

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/non-newtonian-model-identification.git
   cd non-newtonian-model-identification
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the script:
   ```bash
   python model_identification.py
   ```
2. Enter the stress values when prompted, separated by spaces (e.g., `7 8.74 10.14`).
3. Enter the corresponding strain values, separated by spaces (e.g., `1 2 3`).

The program will output:
- Model parameters for each of the three models.
- R² values for model evaluation.
- The name of the best-fit model.

It will also display a plot comparing the experimental data with model predictions.

## Example

**Input:**
```
Enter the stress values separated by spaces (e.g., 7 8.74 10.14):
7 8.74 10.14 11.32 12.33 13.20 14.68 16.03
Enter the corresponding strain values separated by spaces (e.g., 1 2 3):
1 2 3 4 5 6 8 10
```

**Output:**
```
Model fitting results:
Power-Law Model: k = 1.2345, n = 0.8765, R^2 = 0.9876
Bingham Plastic Model: tau0 = 1.2345, eta = 2.3456, R^2 = 0.9543
Herschel-Bulkley Model: tau0 = 1.1234, k = 1.5432, n = 0.7654, R^2 = 0.9987
Best Model: Herschel-Bulkley
```

A plot will also be displayed showing the experimental data and the model predictions.

## File Structure
```
.
├── model_identification.py  # Main script
├── requirements.txt         # Dependencies
├── README.md                # Project documentation
```

## Contributing

Contributions are welcome! If you find any issues or want to enhance the project, feel free to open an issue or create a pull request.


