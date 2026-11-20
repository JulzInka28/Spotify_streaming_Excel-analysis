# Spotify_streaming_Excel-analysis
Interactive Excel dashboard analyzing personal Spotify streaming habits, peak listening, and shuffle skip rates for the period between 2013 and 2023
<img width="1152" height="525" alt="dashboard_preview" src="https://github.com/user-attachments/assets/58c7a5c9-9051-43f0-87ab-a275945424f0" />
[Spotify_Streaming_Analysis.xlsx](https://github.com/user-attachments/files/35118259/Spotify_Streaming_Analysis.xlsx)

## Project Overview
Music Streaming Platforms rely heavily on personalized algorithms and playback features to retain users. In this project, I analysed 149,860 personal streaming records using **Microft Excel**, **Power Query**, and *Power Pivot** to uncover listening habits, peak engagement windows, and playback modes like shuffle impact user skip rates.
## Business Questions Answered 
**Time Intelligence:** Which hours of the day and days of the week drive the highest streaming activity?
**Algorithm & Feature Impact:** Does enabling shuffle mode increase skip rates compared to normal sequential playback?
** Platform Breakdown:** How do listening behaviors differ across devices (android, cast to devide, iOS, mac, web player, windows)?

## Tools & Techniques Workflow
* **Data Cleaning & Transformation (Power Query):**) 
* Converted raw millisecond durations (`ms_played`) into readable mimutes.
* Standardized UTC timestamps into local `Date/Time` formats and engineered custom time-intelligence columns (`Hours`, `Day name`, `Month`)]
* **Data Modeling & DAX (Power Pivot):**
  * Loaded cleaned data into Excell Data Model to optimize performance.
  * Authored custom DAX measures for **Total Hours**, **Skip Rate (%)**, and **Qualifying Streams** (`ms_played >=30000`).
* **Interactive Visualization (Excel Dashboard):**
  * Built a dark-themed, spotify-inspired dashboard utilizing Data Model Pivot Tables, dynamic KPI cards, and custom-styled slicers connected across visuals.
    
## Key Insights & Findings
* **Overall Engagement:** Logged 5,342 hours of total listening across 94,200 qualifying streams, with an average stream rate of 5,25%.
* **The :shuffle Effect":** Tracks played on Shuffle had a 5.57% skip rate compared to 4.32% during normal playback, indicating higher listener friction when relying on randomized queues.
* **Peak Listening windows:** Streaming activity peaked between 5:00 PM and 6:00 PM, aligning closely with after-work hours.
* **Listening volume**:** listening volume was highest on **Friday**
## Strategic Recommendations
**Optimize shuffle weighting**: **Prioritize high-completion tracks and familiar artists queues during peak windows to minimize immediate skips.

## Repository Contents
* `Spotify_Streaming_Analysis.xlsx` - Complete Excel workbook containing Power Query transformations, Power Pivot Data Model, and interactive dashboard.
* `dashboard_preview.png` - High resolution screenshot of the final dashboard.
