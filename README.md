Sales Performance Dashboard (Power BI)

An interactive Power BI report that analyzes $80.45M in sales across product categories, territories, regions and resellers, with slicers for fast filtering.

[Dashboard preview](images/dashboard-preview.png)

Overview

This dashboard answers a few core business questions:

- How much revenue is generated, and how does it compare with cost and tax?
- Which product categories drive sales?
- Which countries, regions and resellers contribute the most?
- How do order quantity and unit price relate to sales across years and categories?

Key metrics

| Metric | Value |
|---|---|
| Sales Amount | $80.45M |
| Total Product Cost | $79.98M |
| Tax Amount | $6.44M |
| Sum of Unit Price | $27.05M |

Dashboard contents

- KPI cards: sales amount, total product cost, tax amount and summed unit price.
- Sales by Product Category (bar chart): compares Bikes, Components, Clothing and Accessories.
- Order Quantity, Unit Price and Sales Amount by Year and Category (scatter chart): shows how volume, price and revenue relate over time.
- Sales by Sales Territory Country (map): geographic spread of sales.
- Sales by Region and Reseller (treemap): top resellers within each region, filtered to resellers above $650,000 in sales.
- Slicers: Product Subcategory, Product Category, Country, Region and Product Name.

Key insights

- Bikes dominate revenue. At about $66M, Bikes account for roughly 82% of the $80.45M total.
- Components are a distant second at about $12M, while Clothing (about $2M) and Accessories (about $1M) contribute little.
- Large resellers are spread across several regions, including Canada, Northwest, Southwest, Southeast, Northeast and Central.
- Higher-revenue points in the scatter chart are mostly Bikes, which suggests that high unit prices, not just volume, drive the category's lead.

Data and tools

- Data source: AdventureWorks
- Tools: Power BI Desktop, Power Query (data cleaning and transformation), data modelling
- Key measures:
  - SalesAmount: total sales revenue
  - TotalProductCost: total cost of the products sold
  - TaxAmt: total tax amount
  - UnitPrice: summed unit price
  - OrderQuantity: number of units ordered, used in the scatter chart alongside UnitPrice and SalesAmount

Repository structure

```
├── sales-dashboard.pbix     # Power BI report file
├── sales-dashboard.pdf      # PDF export of the report
├── images/
│   └── dashboard-preview.png
└── README.md
```

How to open

1. Download `sales-dashboard.pbix` from this repository.
2. Open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows).
3. If prompted, update the data source path or credentials in Transform data → Data source settings.

Don't have Power BI? View the PDF export or the preview image above.

Limitations and future work

- Figures reflect the dataset used for this project and are not live business data.
- Dollar figures are rounded in the visuals, so category totals may not sum exactly to the headline number.
- Planned improvements: add a monthly or yearly sales trend, replace the summed unit price with average unit price, add profit margin analysis, and upgrade the map visual to Azure Maps.

Author

Olaogun Gabriel Olatunji
CS graduate and Research Assistant, LAUTECH
[GitHub](https://github.com/your-GabrielDeAnalyst)
