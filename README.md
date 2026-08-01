Project Overview:

The scope of this assignment was to analyse a large retail dataset and extract useful insights and business value to support decision-making.
The dataset include POS data gathered from cashiers in grocery stores.
For this project the data was was cleaned and visualized using Excel Rapid Miner.

Data Cleaning and Preparation:

Sum Values and Sum Units Data Cleaning:

General Data Cleaning:
Removed invalid basket ids that had n/a in their description.
Deleted barcodes under 12 digits.
Removed negative sum units and values.

Card id Data Cleaning:
Made sure there were no duplicates.
Removed card_id where no card info was provided this was done because for those invalid card ids 72% of the data in the age column was null or blank data. When removed, that % decreased to 35%.

Age Data Cleaning:
Changed the NULL ages to the median of the age column which was 46.

Excel Methodologies :
CONCAT used to merge multiple fields into single identifiers.
VLOOKUP applied to match categories and link external data.
IFERROR used to clean lookup errors and ensure consistency.  Pivot Tables structured transactions into basket-category format.
Converted categories into binary (0/1) for clustering.
Removed duplicates and standardized fields for clean analysis.

Rapid Miner Methodologies:

Used 'Change Role' to assign Basket_ID as ID and keep categories as attributes.
Applied K-Means algorithm for customer and basket segmentation.
Used Clustering operator to generate cluster assignments and centroids.
Visualized cluster patterns using Horizontal BarChart
Ensured accurate clustering by selecting only relevant product-category variables.
