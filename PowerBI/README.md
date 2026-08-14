# Power BI Portfolio

A collection of interactive Power BI projects focused on transforming large, complex datasets into decision-oriented dashboards.

These projects demonstrate experience with **Power BI, Power Query, DAX, data modeling, data validation, interactive reporting, geographic analysis, financial analytics, and executive-level dashboard design**.

---

# 🚕 NYC Yellow Taxi Mobility Intelligence

**File:** `NYC Yellow Taxi Dashboard.pbix`

An end-to-end Power BI analytics project built from **2025 NYC Yellow Taxi trip data**, covering approximately **49 million trip records**.

The dashboard goes beyond basic trip reporting to examine **mobility patterns, geographic flows, congestion, fare economics, passenger behavior, and data quality** across New York City's taxi network.

## Dashboard Pages

### 1. Executive Overview

A high-level view of NYC taxi activity and operating performance.

Includes:

* Clean trip volume
* Revenue
* Average trip distance
* Average travel speed
* Month-over-month performance
* Monthly demand and revenue trends
* Day-of-week × hour demand heatmap
* Pickup borough performance
* Zone performance analysis
* Data quality distribution
* Dynamic business insights

Interactive metric selectors allow users to switch between measures such as:

* Trips
* Revenue
* Trip distance
* Average speed
* Revenue per trip

---

### 2. Movement Explorer

A geographic analysis of pickup and destination behavior across NYC.

Includes:

* Custom NYC Taxi Zone map
* Pickup and dropoff perspectives
* Dynamic location metrics
* Top pickup and destination zones
* Borough-to-borough movement matrix
* Airport trip activity
* Zone performance rankings
* Dynamic movement insights

A custom **TopoJSON NYC Taxi Zone map** is used to visualize activity at the taxi-zone level.

---

### 3. Time & Congestion Intelligence

Analyzes how taxi demand and travel conditions change throughout the day and week.

Includes:

* Hourly demand profile
* Average speed by hour
* Demand versus travel-speed indexing
* Weekday versus weekend speed patterns
* Day × hour congestion heatmap
* Trip duration distribution
* Travel speed by time period
* Highest congestion-pressure zones
* Dynamic congestion insights

The dashboard includes a custom congestion pressure metric combining **relative trip demand and travel speed** to identify periods where high demand coincides with slower movement.

---

### 4. Fare & Passenger Economics

Examines the financial and passenger-side economics of NYC taxi trips.

Includes:

* Total revenue
* Revenue per trip
* Average fare
* Tip rate
* Average trip distance
* Payment method mix
* Recorded tipping behavior
* Monthly revenue composition
* Zone revenue efficiency
* Passenger-count distribution
* Revenue per mile by passenger group
* Airport trip economics
* Dynamic fare and passenger insights

Revenue composition separates components such as:

* Fare revenue
* Tips
* Tolls
* Extra charges
* Congestion surcharges
* Airport fees

---

### 5. Data Quality & Anomaly Review

A dedicated validation layer designed to demonstrate that the underlying data was assessed before being used for business reporting.

Trip records are classified into categories including:

* Valid
* Negative financial value
* Zero distance
* Invalid duration
* Extreme distance
* Extreme fare
* Invalid location

The page includes:

* Total, clean, and flagged trip counts
* Clean and flagged record rates
* Revenue associated with flagged records
* Anomaly distribution
* Anomaly severity review
* Monthly quality trends
* Geographic anomaly patterns
* Hourly flag rates
* Highest anomaly-rate taxi zones
* Dynamic data-quality insights

Rate-based zone rankings use a **minimum trip-volume threshold** to prevent very small samples from creating misleading anomaly rankings.

## Data Preparation & Modeling

The project combines the twelve monthly 2025 Yellow Taxi trip files into a centralized trip fact table.

Major preparation steps include:

* Combining monthly Parquet files
* Correcting column data types
* Restricting analysis to 2025 pickup dates
* Creating trip duration fields
* Creating date, hour, month, day, and time-period attributes
* Building pickup and dropoff taxi-zone dimensions
* Creating a dedicated Date dimension
* Establishing one-to-many dimensional relationships
* Creating data-quality classifications
* Developing reusable DAX measures
* Building custom field parameters for metric switching
* Creating minimum-volume safeguards for rate-based rankings

## Data Model

The model follows a dimensional structure centered on the trip fact table, including:

* `FactTrips`
* `DimDate`
* `DimPickupZone`
* `DimDropoffZone`
* `_Measures`

This structure supports independent pickup and destination analysis while maintaining a centralized measure layer.

## Selected DAX & Analytical Features

Examples include:

* Valid and flagged trip measures
* Revenue per trip
* Revenue per mile
* Average speed
* Tip rate
* Month-over-month comparisons
* Airport trip analysis
* Dynamic metric selection
* Congestion pressure scoring
* Zone rankings
* Data-quality rates
* Dynamic narrative insights

## Data Source

**NYC Taxi & Limousine Commission — Yellow Taxi Trip Records, 2025**

Taxi-zone lookup and geographic boundary data were also used to support zone-level geographic analysis.

## Skills Demonstrated

`Power BI` `Power Query` `DAX` `Data Modeling` `Data Validation` `Data Visualization` `Geospatial Analysis` `Business Intelligence` `Data Storytelling` `Large Dataset Analytics`

---

# 📈 U.S. Treasury Capital Markets Command Center

**File:** `Treasury Capital Markets Command Center.pbix`

An interactive Power BI dashboard analyzing **U.S. Treasury auction activity, investor demand, issuance trends, yields, and market structure**.

The project is designed as a capital-markets command center that allows users to examine Treasury issuance and auction behavior across time and security categories.

## Treasury Market Overview

The primary dashboard provides an executive view of Treasury auction activity.

### Key Performance Indicators

The dashboard tracks:

* **Total Offering**
* **Auction Count**
* **Demand Coverage**
* **Indirect Bidder Share**
* **Weighted High Yield**

These measures provide a compact summary of Treasury issuance scale, auction demand, investor participation, and pricing.

## Treasury Issuance & Investor Demand

A combined annual analysis compares:

* Treasury offering volume
* Auction demand coverage

This makes it possible to examine how investor demand behaves alongside changes in issuance activity.

---

## Investor Participation Mix

Tracks annual accepted-bid participation from:

* Indirect bidders
* Primary dealers
* Direct bidders

This provides visibility into the composition of demand and how participation across investor groups changes over time.

---

## Issuance by Security Type

Compares Treasury offering volume across security groups, allowing users to evaluate differences in issuance activity between Treasury instrument categories.

---

## Treasury Demand by Security Group

Compares average demand coverage across Treasury security groups.

This provides a relative view of investor demand across different types of Treasury securities.

---

## Weighted High Yield by Security Group

Compares offering-weighted auction yields across security categories.

This helps connect Treasury issuance activity with auction pricing and yield behavior.

---

## Interactive Filtering

The dashboard includes interactive controls for:

* **Year**
* **Security Group**

A reset control allows users to clear report filters and return to the default market view.

Visual interactions allow selections to propagate across the dashboard for exploratory analysis.

---

## Model Validation

A dedicated validation page is included to verify core historical and upcoming-auction calculations before they are used in the primary dashboard.

Validation metrics include:

* Total Offering
* Auction Count
* Latest Historical Auction
* Upcoming Offering
* Upcoming Auction Count

This separates model verification from the executive-facing reporting layer and provides an additional quality-control step.

---

## Analytical Focus

The Treasury dashboard is designed to answer questions such as:

* How has Treasury issuance changed over time?
* How does auction demand compare with changes in offering volume?
* Which Treasury security categories account for the greatest issuance?
* How does demand coverage differ across security types?
* How has the mix of indirect bidders, primary dealers, and direct bidders changed?
* How do weighted auction yields vary across Treasury security categories?
* What historical and upcoming auction activity is represented in the model?

## Skills Demonstrated

`Power BI` `DAX` `Power Query` `Financial Analytics` `Capital Markets` `Data Modeling` `Time-Series Analysis` `Interactive Dashboards` `Data Validation` `Executive Reporting`

---

# 🛠️ Tools & Technologies

Across these projects:

| Tool / Skill             | Application                                                           |
| ------------------------ | --------------------------------------------------------------------- |
| **Power BI Desktop**     | Dashboard development and interactive reporting                       |
| **Power Query**          | Data ingestion, transformation, and preparation                       |
| **DAX**                  | Measures, KPIs, rankings, time intelligence, and dynamic calculations |
| **Dimensional Modeling** | Fact and dimension table architecture                                 |
| **Field Parameters**     | Dynamic metric and perspective switching                              |
| **Geospatial Data**      | NYC taxi-zone mapping and location intelligence                       |
| **Data Validation**      | Identification and treatment of anomalous records                     |
| **Git & Git LFS**        | Version control and storage of large `.pbix` files                    |
| **GitHub**               | Project documentation and portfolio presentation                      |

---

# 📂 Files

```text
PowerBI/
├── NYC Yellow Taxi Dashboard.pbix
├── Treasury Capital Markets Command Center.pbix
└── README.md
```

The `.pbix` files can be opened using **Microsoft Power BI Desktop**.

> **Note:** The NYC Yellow Taxi dashboard contains a large imported dataset and is stored using Git Large File Storage (Git LFS). Downloading the complete project may therefore require additional time.

---

# 💡 Project Approach

My goal with these projects was not simply to create charts, but to build analytical products that support exploration and decision-making.

The projects emphasize:

* Clear business questions
* Reliable data preparation
* Structured dimensional models
* Reusable analytical measures
* Interactive exploration
* Appropriate handling of anomalies and edge cases
* Executive-level visual storytelling
* Detailed analytical views for deeper investigation

The NYC project demonstrates large-scale operational and geographic analytics, while the Treasury project demonstrates financial-market analysis and executive reporting.

Together, they showcase the ability to translate complex datasets into structured, interactive business intelligence solutions.
