# Social Media Analytics Dashboard – Data Documentation

## Data Overview

This dashboard analyzes social media performance across platforms on a monthly basis. Data is collected for a full year, with each row representing a post’s performance metrics for a specific month and platform.

---

## Data Sources and Storage

- **Platforms:** YouTube, Facebook (add more as included)
- **Data Extraction:** Data can be exported from platform analytics or via APIs.
- **Storage Format:**  
  - For small/medium data: Excel (.xlsx) or CSV (.csv) files
  - For large data: Stored and queried via SQL databases

---

## Data Structure

The core dataset has the following columns:

| Column           | Description                                                     |
|------------------|-----------------------------------------------------------------|
| Month            | Month and year of the data entry (e.g., 01 August 2024)         |
| Platform         | Social media platform (YouTube, Facebook, etc.)                 |
| Post ID          | Unique identifier for each post                                 |
| Post Type        | Type of post (e.g., Video, Image, etc.)                         |
| Reach            | Number of unique users who saw the post                         |
| Impressions      | Total number of times the post was displayed                    |
| Likes            | Total likes or reactions                                        |
| Comments         | Number of comments                                              |
| Shares           | Number of times post was shared/retweeted                       |
| Saves            | Number of times post was saved/bookmarked (if available)        |
| Clicks           | Total clicks on the post/link                                   |
| New Followers    | Followers gained attributable to the post                       |
| Total Followers  | Total followers at the time of posting                          |
| Engagement Rate  | Calculated field: (Likes + Comments + Shares) / Total Followers (as defined in the dashboard) |

> *Sample data table as visualized in Power BI.*
> <img width="1609" height="685" alt="Screenshot 2025-08-03 101825" src="https://github.com/user-attachments/assets/1d098a57-6a66-4a43-8cda-7aadb52e2f49" />
> <img width="1609" height="685" alt="image" src="https://github.com/user-attachments/assets/fe986e30-cb64-401f-a9e3-58bbe9f90687" />

---

## Data Usage

- **Power BI Dashboard:** Data is imported into Power BI for visualization and analysis.
- **Calculated Metrics:** Engagement Rate and other KPIs are calculated within Power BI or in the source data file.
- **Refresh Process:**  
  - For Excel/CSV: Replace or append new data and refresh Power BI.
  - For SQL: Data is updated in the database; Power BI queries the latest data.

---

## Data Preparation Notes

- **Consistency:** Ensure date formats and column names are consistent across months and platforms.
- **Cleaning:** Remove duplicates, fill missing values, and standardize metrics where necessary.
- **Scalability:** For larger data, consider migrating to an SQL database for faster queries and automation.

---

## Example Usage

To update the dashboard:
1. Export the latest monthly data from each platform.
2. Append to the existing Excel/CSV file or import into SQL table.
3. Open Power BI and refresh the dataset to update visuals.

---

## Security & Privacy

- Data files should be stored securely and access should be controlled.
- Personal data should be anonymized or handled according to privacy regulations.

---

## License

MIT

