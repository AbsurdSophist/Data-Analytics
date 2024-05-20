# Crypto Arbitrage Opportunity Analysis

## Overview
This repository contains a Jupyter Notebook designed to analyze arbitrage opportunities in the cryptocurrency market. Arbitrage involves exploiting price differences of the same asset in different markets. The analysis is performed using data imported from CSV files, with the goal of identifying profitable trading opportunities by comparing prices across various exchanges.

## Project Structure

```
Crypto-Arbitrage-Analysis/
├── Resources/
│   ├── bitstamp.csv
│   ├── coinbase.csv
├── Crypto_Arbitrage_Analysis.ipynb
├── README.md
└── LICENSE
```

### Directories and Files

- **Resources/**: Contains the raw CSV files with price data from different cryptocurrency exchanges.
  - `bitstamp.csv`: Price data from Bitstamp.
  - `coinbase.csv`: Price data from Coinbase.

- **Crypto_Arbitrage_Analysis.ipynb**: Jupyter Notebook that contains the code for data preprocessing and arbitrage analysis.

- **README.md**: This readme file, providing an overview of the project and instructions for use.

- **LICENSE**: The license under which the project is released.

## Getting Started

### Prerequisites

Ensure you have Python 3.8 or higher and Jupyter Notebook installed on your system. Additionally, you will need to install the necessary Python packages. It is recommended to use a virtual environment to manage dependencies.

### Installation

1. **Clone the repository:**

   ```bash
   git clone git@github.com:AbsurdSophist/Data-Analytics-and-Visualizations.git
   cd Crypto-Arbitrage-Analysis
   ```

2. **Create a virtual environment and activate it:**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install the required packages:**

   You can install the necessary packages using `pip`:

   ```bash
   pip install pandas jupyter
   ```

### Usage

1. **Add your data files:**
   
   Place your CSV files containing cryptocurrency prices into the `Resources/` directory. Ensure the filenames match those referenced in the notebook or update the file paths in the notebook accordingly.

2. **Run the Jupyter Notebook:**

   Start the Jupyter Notebook server and open the `Crypto_Arbitrage_Analysis.ipynb` file.

   ```bash
   jupyter notebook
   ```

3. **Execute the Notebook Cells:**

   Follow the steps in the notebook to preprocess the data and analyze arbitrage opportunities. The notebook includes code cells for:
   - Loading and inspecting the data.
   - Cleaning and preprocessing the data.
   - Analyzing price differences to identify arbitrage opportunities.

## Findings

After collecting and preparing the historical data from each exchange, we focused on specific time periods. We selected three arbitrary dates from each year for which data was available (2016, 2017, and 2018). The analysis revealed the following:

- **2016 and 2017:** Significant arbitrage opportunities were identified in these years. The plots generated show notable price differences between exchanges, suggesting multiple opportunities for profitable trades.
- **2018:** The data showed consistent pricing across exchanges, resulting in sparse and less profitable arbitrage opportunities.

We further refined the analysis by targeting opportunities where the profit margin was at least 1%. This allowed us to calculate the total potential profit for each analyzed day. While both 2016 and 2017 had numerous opportunities exceeding a 1% profit margin, the absolute profit was much higher in 2017 due to the substantial increase in Bitcoin's price, which rose from hundreds of dollars in 2016 to thousands in 2017. 

In contrast, 2018 showed virtually no viable arbitrage opportunities, questioning the future profitability of this strategy.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure your code follows the project's style guidelines and includes appropriate tests.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact

For any questions or inquiries, please contact [Lucas Manning](mailto:AbsurdSophist@gmail.com).

---

Thank you for exploring this project. Happy trading!