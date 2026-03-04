# Bitcoin Transaction Network Analysis

An analysis of the Elliptic Bitcoin transaction dataset using NetworkX to understand blockchain network topology, identify patterns in illicit vs licit transactions, and characterize the structure of the Bitcoin transaction graph.

## Dataset

The ([https://www.kaggle.com/datasets/ellipticco/elliptic-data-set](https://www.kaggle.com/code/artgor/elliptic-data-eda)) contains:
- **203,769** Bitcoin transactions
- **234,355** transaction flows (edges)
- Transaction labels: licit (1), illicit (2), unknown

## Analysis Performed

- **Graph Construction**: Built directed transaction graph from edge list
- **Degree Analysis**: Computed in-degree, out-degree, and total degree distributions
- **Centrality Measures**: Identified most connected nodes (potential exchanges/mixers)
- **Clustering**: Calculated average clustering coefficient (0.0132)
- **Component Analysis**: Identified 49 weakly connected components
- **Class Comparison**: Compared behavioral patterns between licit and illicit transactions

## Key Findings

| Metric | Value |
|--------|-------|
| Total Transactions | 203,769 |
| Total Flows | 234,355 |
| Network Density | 0.00000564 |
| Average Degree | 2.30 |
| Max Degree | 473 (likely exchange/mixer) |
| Clustering Coefficient | 0.0132 |
| Licit Transactions | 4,545 |
| Illicit Transactions | 42,019 |
| Illicit Avg Degree | 3.10 (53.9% higher than licit) |

## Key Insight

Illicit transactions show **53.9% higher average connectivity** than licit transactions, suggesting mixing/obfuscation behavior common in money laundering.

## Requirements
networkx
pandas
matplotlib
numpy
seaborn
jupyter


## Usage

1. Clone this repository
2. Install requirements: `pip install -r requirements.txt`
3. Download the Elliptic dataset from Kaggle
4. Update file paths in the notebook to point to your data
5. Run the notebook


## Re
