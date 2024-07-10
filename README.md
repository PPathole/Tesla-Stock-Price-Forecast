# Tesla Stock Price Prediction

This project uses historical stock data of Tesla (TSLA) to predict future stock prices using a linear regression model. The data is fetched using the `yfinance` library, and the predictions are visualized using Matplotlib.

## Table of Contents

- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Feature Engineering](#feature-engineering)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Visualization](#visualization)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to predict Tesla's stock prices using historical data. It leverages Python's machine learning libraries to train a linear regression model and visualize the results.

## Data Collection

We use the `yfinance` library to download Tesla's historical stock data. The data includes the following columns:
- Date
- Open
- High
- Low
- Close
- Volume
- Dividends
- Stock Splits

## Feature Engineering

Additional features are created to help the model better understand temporal patterns:
- Year
- Month
- Day
- Day of the Week
- Volume

## Model Training

The data is split into training and testing sets using `train_test_split` from `sklearn.model_selection`. A linear regression model is then trained on the training set.

## Evaluation

The model's performance is evaluated using Mean Squared Error (MSE) and R^2 Score. These metrics are printed out after the model training:

```plaintext
Mean Squared Error: 3838
R^2 Score: 0.6384
```

## Visualization

The results are visualized using Matplotlib. The plot includes:
- Historical stock prices (solid blue line)
- Predicted stock prices (dotted red line)

The plot helps in understanding how well the model's predictions match the actual stock prices.

## Usage

To run this project, you need to have Python installed along with the following libraries:
- yfinance
- pandas
- numpy
- matplotlib
- scikit-learn

You can install the required libraries using:
```bash
pip install yfinance pandas numpy matplotlib scikit-learn
```

### Running the Script

1. Clone the repository:
    ```bash
    git clone <repository_url>
    ```
2. Navigate to the project directory:
    ```bash
    cd tesla-stock-price-prediction
    ```
3. Run the script:
    ```bash
    python predict_tesla_stock.py
    ```

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
