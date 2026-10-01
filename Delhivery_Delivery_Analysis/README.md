# 🚚 Delhivery: Logistics Delivery Analysis & Strategy Building

## Dataset:Columns
* •	data - tells whether the data is testing or training data
* •	trip_creation_time – Timestamp of trip creation
* •	route_schedule_uuid – Unique Id for a particular route schedule
*•	route_type – Transportation type
* o	FTL – Full Truck Load: FTL shipments get to the destination sooner, as the truck is making no other pickups or drop-offs along the way
* o	Carting: Handling system consisting of small vehicles (carts)
* •	trip_uuid - Unique ID given to a particular trip (A trip may include different source and destination centers)
* •	source_center - Source ID of trip origin
* •	source_name - Source Name of trip origin
* •	destination_cente – Destination ID
* •	destination_name – Destination Name
* •	od_start_time – Trip start time
* •	od_end_time – Trip end time
* •	start_scan_to_end_scan – Time taken to deliver from source to destination
* •	is_cutoff – Unknown field
* •	cutoff_factor – Unknown field
* •	cutoff_timestamp – Unknown field
* •	actual_distance_to_destination – Distance in Kms between source and destination warehouse
* •	actual_time – Actual time taken to complete the delivery (Cumulative)
* •	osrm_time – An open-source routing engine time calculator which computes the shortest path between points in a given map (Includes usual traffic, distance through major and minor roads) and gives the time (Cumulative)
* •	osrm_distance – An open-source routing engine which computes the shortest path between points in a given map (Includes usual traffic, distance through major and minor roads) (Cumulative)
* •	factor – Unknown field
* •	segment_actual_time – This is a segment time. Time taken by the subset of the package delivery
* •	segment_osrm_time – This is the OSRM segment time. Time taken by the subset of the package delivery
* •	segment_osrm_distance – This is the OSRM distance. Distance covered by subset of the package delivery
* •	segment_factor – Unknown field


## 📌 Project Overview
Delhivery is India's largest fully integrated logistics services provider. To maintain high efficiency and outpace competitors, the company relies heavily on data-driven intelligence to forecast delivery times, optimize shipping routes, and minimize delays between warehouses and final destinations.

The objective of this project is to clean, process, and analyze raw logistics data from Delhivery. By engineering key features and analyzing delivery time gaps, this study provides actionable strategic recommendations to optimize transit operations and improve supply chain predictability.

---

## 🚀 Key Analysis Frameworks & Strategy Blocks

### 1. Data Cleaning & Structuring
▪️ **Handling Aggregated Data:** Managing raw telemetry logs by parsing and reconstructing trips from source to destination.
▪️ **Outlier Detection:** Identifying anomalies in distance and time metrics using statistical techniques (IQR) to flag exceptional delays.
▪️ **Missing Value Imputation:** Resolving missing data elements in spatial and temporal features to ensure data integrity.

### 2. Feature Engineering & Discrepancy Analysis
🟢 **Time Gaps:** Analyzing the variance between Actual Transit Time and the Open Source Routing Machine (OSRM) predicted time.
🟡 **Distance Gaps:** Comparing actual kilometers traveled against OSRM-computed shortest paths to track routing inefficiencies.
🔵 **Categorical Engineering:** Grouping delivery points by state, city tiers, and route types (FTL vs. Carting) to pinpoint structural bottlenecks.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Data Manipulation:** `pandas` (Grouping, aggregations, datetime parsing, data type conversions), `numpy`
* **Data Visualization:** `seaborn`, `matplotlib` (Distribution plots, box plots for outlier tracking)
* **Statistical Analysis:** Hypothesis testing (ks_2samp) to validate differences between actual_distance and estimated_distance

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd delhivery-delivery-analysis
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter framework to explore the full analysis and strategic takeaways:
```bash
jupyter notebook Delhivery_Case_Study.ipynb
```

