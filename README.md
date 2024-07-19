# Ethereum Weekly Transaction Data Analysis

This repository contains an analysis of a week's worth of Ethereum transaction data. The analysis includes various advanced visualizations to uncover insights and trends in the transaction data.

## Overview

The Ethereum network is a leading platform for decentralized applications and smart contracts, resulting in significant transaction volume and value. This analysis examines a week's worth of Ethereum transaction data, providing insights through various advanced data visualizations.

## Data

The dataset includes the following fields for each transaction:
- `tx_hash`: Transaction hash
- `block_number`: Block number
- `timestamp`: Timestamp of the transaction
- `from`: Sender's address
- `to`: Receiver's address
- `value`: Transaction value in Ether

## Visualizations

### Scatter Plot

![Scatter Plot](scatter_plot.png)

The scatter plot displays Ethereum transactions over a week, with transaction values color-coded for clarity. Each point represents a transaction, with its timestamp on the x-axis and transaction value on the y-axis.

**Insights:**
- **Transaction Distribution:** Transactions are evenly distributed throughout the week, indicating consistent network activity.
- **Value Range:** Transaction values range from 0.5 to 5 Ether, showcasing the diversity in transaction sizes.
- **Clustering:** Higher transaction values appear to be more clustered around specific times, possibly reflecting peak usage periods or significant network events.

### Bubble Chart

![Bubble Chart](bubble_chart.png)

The bubble chart represents transactions with bubble sizes proportional to the block number. This visualization helps identify periods of higher block activity.

**Insights:**
- **Activity Peaks:** Larger bubbles indicate higher block numbers, suggesting more activity during these periods.
- **Value Correlation:** There is a noticeable trend where higher transaction values coincide with higher block numbers, potentially indicating busier network periods.

### Pair Plot

![Pair Plot](pair_plot.png)

The pair plot examines relationships between block numbers and transaction values, with transactions color-coded by value.

**Insights:**
- **Positive Correlation:** There is a positive correlation between block number and transaction value, indicating that as the block number increases, so do the transaction values.
- **Value Clustering:** Higher transaction values are more concentrated, suggesting fewer high-value transactions compared to lower-value ones.

### Histogram

![Histogram](histogram.png)

The histogram illustrates the distribution of transaction values over the week.

**Insights:**
- **Frequency Distribution:** The majority of transactions are clustered around lower values (0.5 to 2 Ether), indicating smaller, more frequent transactions dominate the network.
- **Value Outliers:** There are fewer high-value transactions, reflecting the occasional nature of large transfers on the network.

### Box Plot

![Box Plot](box_plot.png)

The box plot provides a visual summary of transaction values, highlighting the median, quartiles, and potential outliers.

**Insights:**
- **Median Value:** The median transaction value is around 2 Ether, suggesting a balanced transaction distribution.
- **Outliers:** Several outliers are present, indicating sporadic high-value transactions that deviate significantly from the median.

### Violin Plot

![Violin Plot](violin_plot.png)

The violin plot combines aspects of the box plot and density plot, showing the distribution of transaction values with density estimation.

**Insights:**
- **Value Distribution:** The plot reveals a bimodal distribution with peaks around lower and higher values, suggesting two distinct transaction value groups.
- **Density Peaks:** The highest density of transactions occurs around 1 to 2 Ether, aligning with earlier observations from the histogram.

## Conclusion

The Ethereum transaction data over a week reveals several key insights:
- **Consistent Activity:** The network maintains consistent transaction activity throughout the week.
- **Transaction Value Distribution:** Most transactions are of lower value, with fewer high-value transactions.
- **Correlation with Block Number:** Higher transaction values often coincide with higher block numbers, indicating busier periods on the network.
- **Outliers and Density:** The presence of outliers and the bimodal distribution of values highlight the diversity in transaction sizes and frequency.

These visualizations and insights provide a comprehensive understanding of Ethereum's transaction dynamics, essential for further analysis and decision-making in the context of blockchain data analytics.

## Usage

To reproduce the visualizations, run the provided Python script `eth_analysis.ipynb`. Ensure you have the required libraries installed:

```bash
pip install pandas matplotlib seaborn

Then run/upload the script:

python eth_analysis.ipynb ---> on jupyter notebook


