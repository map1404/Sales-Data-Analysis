# Sales Data Analysis

This project analyzes retail sales data to clean transaction records, engineer customer-level features, segment customers, study purchase patterns, and explore geographic behavior. The analysis is now organized into a clearer notebook-first workflow.

## Project Goals

- Clean and merge raw sales data from multiple source files
- Build customer-level features for behavioral analysis
- Segment customers using clustering techniques
- Analyze market basket patterns and association rules
- Explore geographic trends in store and transaction activity

## Project Structure

The project is organized around these ordered notebooks:

- `01_Initial_Analysis_and_Cleaning.ipynb`
- `02_Feature_Engineering.ipynb`
- `03_EDA.ipynb`
- `04_Customer_Segmentation.ipynb`
- `05_Clustering_Method_Comparison.ipynb`
- `06_Market_Basket_Analysis.ipynb`
- `07_Segment_Association_Rules.ipynb`
- `08_Geographical_Analysis.ipynb`

Supporting folders:

- `dataset/`: raw input CSVs
- `generated/`: generated CSV outputs
- `figures/`: saved charts and figures

## Required Input Files

The notebooks read these raw files from `dataset/`:

- `TOKEN.csv`
- `VENTE.csv`
- `ARTICLE.csv`
- `MAGASIN.csv`

Generated intermediate files written to `generated/` include:

- `merged_transactions.csv`
- `customer_features_prepared.csv`
- `segment_profiles.csv`
- `segment_business_summary.csv`
- `customers_with_segments.csv`

Figures are saved to `figures/`.

## Recommended Execution Order

Run the notebooks in this sequence:

1. `01_Initial_Analysis_and_Cleaning.ipynb`
2. `02_Feature_Engineering.ipynb`
3. `03_EDA.ipynb`
4. `04_Customer_Segmentation.ipynb`
5. `05_Clustering_Method_Comparison.ipynb`
6. `06_Market_Basket_Analysis.ipynb`
7. `07_Segment_Association_Rules.ipynb`
8. `08_Geographical_Analysis.ipynb`

## Python Libraries

The notebooks use the following main packages:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`
- `mlxtend`
- `folium`
- `networkx`

Install them with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy mlxtend folium networkx jupyter
```

## Outputs

Depending on which notebooks you run, the project can generate:

- cleaned and merged transaction data
- customer feature tables for clustering
- customer segment assignments and profile summaries
- association rule reports for all customers and per segment
- top-product and cross-sell recommendation tables
- visualizations for segmentation, basket analysis, and geography

## Notes

- Some notebooks depend on outputs created by earlier notebooks, so running them out of order may cause missing-file errors.
- The numbered notebooks are intended to run from the `Sales-Data-Analysis` folder so their relative paths resolve to `dataset/`, `generated/`, and `figures/`.
- Notebook-only lines such as `!pip install ...` were converted into comments in the structured notebooks.
