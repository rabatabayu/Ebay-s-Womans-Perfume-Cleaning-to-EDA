# eBay Women's Perfume — Data Cleaning & Sales Analytics

## Project Overview
This project focuses on cleaning and analyzing eBay women's perfume listing data using Python. The goal is to understand product performance, pricing patterns, and customer demand indicators to support data-driven decisions on product selection, pricing, and inventory planning.

## Objectives
- Prepare a consistent, analysis-ready dataset by addressing missing values, duplicates, and inconsistent formats.
- Identify leading perfume brands, product types, and individual listings based on reported units sold.
- Explore price distributions and the relationship between listed price and units sold.
- Translate exploratory findings into practical business recommendations.

## Dataset Overview
The dataset contains eBay perfume listings with information such as:

| Field | Description |
| --- | --- |
| `brand` | Perfume brand |
| `title` | Product or listing name |
| `type` | Perfume category (e.g., EDP, EDT, EDC) |
| `priceWithCurrency` | Listed price before numeric conversion |
| `availableText` | Text describing available inventory |
| `sold` | Reported number of units sold |
| `itemLocation` | Seller or item location |

**Note:** This is listing-level marketplace data. Reported units sold are not the same as verified company transactions, and the dataset does not establish causation or a time-series sales trend.

## Tools & Libraries
- **Python** — data cleaning and exploratory analysis
- **Pandas & NumPy** — data manipulation and numerical analysis
- **Matplotlib & Seaborn** — data visualization
- **Jupyter Notebook** — analysis documentation and execution

## Project Workflow

### 1. Data Cleaning
- Checked data types, missing values, and duplicate records.
- Converted price strings into numeric values.
- Extracted numeric availability and sold counts from text where needed.
- Reviewed inconsistent category values and potential outliers.
- Validated the cleaned dataset before analysis.

### 2. Exploratory Data Analysis (EDA)
- **Univariate analysis:** distributions of price, sales, brands, and perfume types.
- **Product performance:** top-selling listings and brands.
- **Category analysis:** total and average units sold by perfume type.
- **Bivariate analysis:** relationship between price and units sold.
- **Multivariate analysis:** correlation heatmaps, pairplots, and grouped comparisons.

## Key Findings

| Area | Finding |
| --- | --- |
| Highest total units sold by type | **Eau de Parfum (EDP): 271,299 units** |
| Highest average units sold per listing | **Eau de Toilette (EDT): approximately 886.64 units** |
| Leading individual listing | **Escape by Calvin Klein: 17,854 reported units sold** |
| Price vs. units sold | **Negative correlation** in the analyzed listings |
| Frequently represented brands | **Dolce & Gabbana (44 listings)** and **Lancôme (41 listings)** |

The results suggest that high-volume product types and individual bestsellers deserve closer attention. The negative price–sales association may also warrant further investigation, but it does not prove that lowering prices will increase demand.

## Business Recommendations
1. **Prioritize proven products:** use high-selling listings and perfume types as inputs to assortment decisions.
2. **Test pricing strategies:** evaluate price bands by product type and brand rather than applying one discount approach to every product.
3. **Improve inventory planning:** combine observed sales activity with availability to identify items that may need closer stock monitoring.
4. **Expand future analysis:** add transaction dates, costs, and customer-level data to measure revenue, profit, retention, and sales trends more reliably.

## Conclusion
Exploratory analysis of eBay perfume listings reveals meaningful differences in sales performance across perfume types, brands, and products. These findings offer an initial basis for more informed pricing, merchandising, and inventory decisions while highlighting the need for richer data before making causal or profitability claims.
