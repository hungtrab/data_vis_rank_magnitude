The video about our making of the project is available at [YouTube](https://youtu.be/sJCJeBEwHy0)

# Mini Project: Data Visualization - Showing Rank and Magnitude

This repository contains the files for our mini-project for the Data Visualization course (IT4023E) at Hanoi University of Science and Technology (HUST).

## Team Members

| Name                         | Student ID |
| ---------------------------- | ---------- |
| Chu Anh Đức            | 20230081    |
| Vũ Thường Tín              | 20230091    |
| Trần Quang Hưng               | 20235502    |
| Đỗ Đăng Vũ              | 20235578    |
| Nguyễn Xuân Khải              | 20235508    |

## Project Overview

The primary goal of this project is to effectively visualize and communicate insights related to **rank and magnitude** within a given dataset. We aim to demonstrate how different products or categories perform relative to each other and showcase their overall sales impact. The dashboard allows users to explore product performance both overall and within specific segments or regions, dynamically highlighting relationships and providing detailed breakdowns.

## Data Visualization (Tableau Workbook)

You can download our Tableau Workbook (`.twb` file) from this repository to explore the visualizations interactively.

**File:** `[Showing_Rank_And_Magnitude.twb]`

### Important Notes for Running the Tableau File:

To ensure the Tableau workbook functions correctly with your data source (if you are connecting it to the original CSV), please pay attention to the following data type configurations within Tableau's Data Source pane:

1.  **`Sales` Column:**
    *   The `Sales` column in your raw data source (CSV) might contain currency symbols (e.g., "$") and thousands separators (e.g., "," or ".").
    *   For our calculations to work (especially for cleaning and converting to a numeric value if needed), ensure that **Tableau initially interprets the `Sales` column from your CSV as a String (Text - "Abc" icon)**.
    *   If you are using a calculated field (e.g., `Sales Numeric`) to convert this string to a measurable numeric value within Tableau (as we discussed), that calculated field should then be a **numeric data type (e.g., Number (decimal) - "#.#" icon)**. The visualizations will use this numeric version for aggregations.

2.  **`Order Date` Column:**
    *   Ensure the `Order Date` column is correctly interpreted by Tableau as a **Date & Time data type (calendar & clock icon)** or at least a **Date data type (calendar icon)**. This is crucial for any time-based analysis or for extracting year/month/day components.


---
