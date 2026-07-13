# nsw-sa2-wellresourced-analysis
NSW Regional Statistics & POI-Based Well-Resourced Scoring

Group project — DATA2001: Data Science, Big Data and Data Variety

Analysed NSW-wide demographic, housing, and business statistics (Task 1), then built a data pipeline using the NSW Points of Interest API to calculate a "well-resourced" score for SA2 regions across four Greater Sydney SA4 zones — Blacktown, North Sydney & Hornsby, Parramatta, and Northern Beaches (Tasks 2–3).

Key finding: While average well-resourced scores were similar across all four SA4 regions (0.48–0.49), each region showed sharp internal variation between its highest- and lowest-scoring SA2 areas — meaning local resource access varies far more within a region than between regions.

My contribution — Sydney-Blacktown region:
- Built the function to extract Points of Interest from the NSW POI API within Blacktown's SA2 bounding boxes
- Ran the extraction loop across all 24 Blacktown SA2 regions and loaded results into the shared SQL database
- Calculated well-resourced scores (z-score standardisation + sigmoid transformation) for each Blacktown SA2
- Built the score distribution histogram and spatial map-overlay visualisation for Blacktown
- Wrote the Blacktown-specific findings section of the final report (Section 3.2)

Tools: Python, Pandas, GeoPandas, SQL (SQLite), NSW POI API, data visualisation
