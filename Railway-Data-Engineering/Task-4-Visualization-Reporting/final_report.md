# Railway Data Engineering Project
## Final Internship Report

### 1. Project Objective
Explore railway records, clean and transform the dataset, analyze
weekly operating patterns, and visualize station and route distributions.

### 2. Dataset Overview
- Total records: 11,113
- Number of columns: 5
- Unique train numbers: 11,113
- Unique source stations: 921
- Unique destination stations: 924
- Missing values in the cleaned dataset: 0
- Exact duplicate rows in the cleaned dataset: 0

### 3. Tools Used
- Python
- Pandas
- Matplotlib
- Jupyter Notebook

### 4. Data Cleaning
Missing values were checked across all columns. No rows required
removal due to missing essential values. Text fields were standardized,
station names converted to uppercase, and weekday labels corrected.
The cleaned dataset was saved separately from the original CSV.

### 5. Data Transformation
The dataset was filtered for Saturday records and for departures
from CHENNAI BEACH. Grouping and aggregation were used to count
records by source station. A weekday/weekend category was also added.

### 6. Weekly Distribution
days
Monday       1503
Tuesday      1628
Wednesday    1612
Thursday     1526
Friday       1649
Saturday     1593
Sunday       1602

- Highest-count day: Friday (1,649 records)
- Lowest-count day: Monday (1,503 records)
- Weekday records: 7,918
- Weekend records: 3,195

### 7. Station Analysis
#### Top 10 Source Stations
Source_Station_Name
CST-MUMBAI       513
SEALDAH          372
CHENNAI BEACH    339
HOWRAH JN.       338
KALYAN JN        285
THANE            186
PANVEL           141
TAMBARAM         140
MOOR MARKET      135
VELACHEERY       115

#### Top 10 Destination Stations
Destination_Station_Name
CST-MUMBAI       514
SEALDAH          373
CHENNAI BEACH    342
HOWRAH JN.       337
KALYAN JN        284
THANE            194
PANVEL           144
TAMBARAM         140
MOOR MARKET      132
VELACHEERY       118

### 8. Visualizations
The project includes the following charts:
1. Daily railway record distribution.
2. Weekday versus weekend record comparison.
3. Top 10 source stations.
4. Source-destination record count heatmap.

Refer to the charts folder for the generated PNG files.

### 9. Key Findings
- CST-MUMBAI is the most frequently recorded source and destination station.
- Friday has the highest number of records among the seven days.
- Monday has the lowest number of records.
- The dataset contains more weekday records than weekend records.
- Route counts are concentrated in particular source-destination pairs.

### 10. Limitations
The dataset contains train records and operating-day labels, not passenger
counts or passenger demand. Record frequency alone cannot establish
capacity requirements or justify changes to railway schedules.
The correlation using a sequential weekday index is descriptive only
and does not demonstrate causation.

### 11. Conclusion
The project demonstrates data loading, quality checks, cleaning,
filtering, aggregation, enrichment, exploratory analysis, and
visualization using Python. The outputs provide a structured summary
of the railway dataset and its recorded operating patterns.
