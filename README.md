Supplier–Warehouse–Shipment–Inspection Data Preview
Overview
This Python script provides a straightforward way to preview key datasets related to a supply chain system involving suppliers, warehouses, shipments, and inspections. It reads four CSV files and displays the first few rows of each, helping users quickly understand the data structure before performing deeper analysis.

Dataset Description
The project uses four separate datasets, each stored as a CSV file:

suppliers.csv: Contains information about suppliers, such as Supplier ID, name, and country.

warehouses.csv: Contains details about warehouses, including Warehouse ID, location, and capacity.

shipments.csv: Records shipments linking suppliers to warehouses, including shipment dates.

inspections.csv: Includes inspection results associated with shipments or suppliers.

Features
Loads datasets using Pandas for efficient data handling.

Displays the first five rows (head) of each dataset to provide an immediate snapshot of the data.

Sets Pandas options to display all columns, ensuring no data is hidden in the preview.

Configures Seaborn and Matplotlib styles for consistent aesthetics (useful if extended for visualization later).

Requirements
Python 3.x

Libraries: numpy, pandas, matplotlib, seaborn

To install dependencies, run:
pip install numpy pandas matplotlib seaborn

How to Use
Ensure the following CSV files are placed in the same directory as the script:
suppliers.csv, warehouses.csv, shipments.csv, inspections.csv

Run the script using:
python preview_datasets.py

The script will output the first five rows of each dataset to the console.

Example Output
Suppliers data
SupplierID | Name | Country
1 | ABC Ltd | Germany
2 | XYZ Inc | USA
...

Warehouses data
WarehouseID | Location | Capacity
10 | Berlin | 15000
...

Shipments data
ShipmentID | SupplierID | WarehouseID | Date
100 | 1 | 10 | 2023-05-14
...

Inspections data
InspectionID | ShipmentID | Status
500 | 100 | Passed
...

Next Steps & Suggestions
Data Cleaning: Handle missing values, fix data types, and check for inconsistencies.

Exploratory Data Analysis (EDA): Generate summary statistics and visualizations to understand trends and relationships.

Integration: Link datasets (e.g., join shipments with suppliers and warehouses) for combined insights.

Reporting: Create dashboards or reports highlighting key performance indicators.

Automation: Expand the script to automatically generate summaries or visualizations after loading data.

