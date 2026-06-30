# StreamFlix Dashboard & Performance Analysis

## Project Introduction
This project provides an end-to-end data analytics solution tracking viewer behaviors, content performance, and subscription analytics for the **StreamFlix** streaming platform. Using an ETL pipeline spanning Python data manipulation, SQL storage, and advanced visualization libraries, this project turns messy interaction data into clean, interactive dashboards.

---

## Data Pipeline & ETL Process
Before generating any visual insights, the raw dataset underwent an extensive **Extract, Transform, Load (ETL)** pipeline using Python:

* **Data Cleansing:** Eradicated structural inconsistencies by systematically cleaning the **Movie Names** and **Genres** columns.
* **Deduplication:** Identified and purged all duplicate entry records to preserve transactional integrity.
* **Outlier Management:** Analyzed numeric distributions for anomalies and removed data outliers distorting the metrics.
* **Type Formatting:** Standardized the **Date** columns into uniform datetime values for accurate time-series evaluation.
* **Database Ingestion:** Connected Python directly to an SQL database infrastructure via an object-relational mapping engine, allowing us to load the cleaned data for secure querying.

---

## Dashboard Visual Snapshots
The project generates six data snapshots to analyze performance across separate operational dimensions:

1. **Top 10 Movies by Average Ratings:** Evaluates content quality and critical acclaim across the media catalog.
2. **User Distribution by Age Group:** Breaks down user demographics to uncover target audience generation brackets.
3. **Top 20 Genres (Deep Dive):** Analyzes total viewership and volume distribution across the top 20 most popular categories.
4. **User Distribution by Country of Origin:** Maps out international subscriber footprints and global viewer density.
5. **Subscription Status Breakdown:** Monitors recurring revenue health by tracking active Free vs. Premium Subscribed profiles.
6. **Device Usage Distribution:** Tracks software and hardware endpoints to pinpoint how users choose to consume media content.

---

## Technical Stack
* **Language:** Python
* **Database Layer:** SQL (`sqlalchemy` for engine creation)
* **Data Manipulation:** Pandas, NumPy
* **Visualization Engine:** `matplotlib.pyplot`, `seaborn`, `matplotlib.colors`
