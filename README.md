# Weather-Dashboard-Automation
Real-time weather dashboard using Power BI and Power Automate
# Weather Dashboard Automation using Power BI & Power Automate

## Overview
This project demonstrates a real-time weather monitoring system using **Power BI**, **Power Automate**, and the **OpenWeatherMap API**. The system fetches weather data twice daily and updates an interactive dashboard with insights for different cities/states.

---

## Tools & Technologies
- **Power BI** – for visualizing real-time weather data.
- **Power Automate** – to schedule API calls and update data automatically.
- **OpenWeatherMap API** – for weather data.
- **Microsoft Excel (OneDrive)** – acts as the data store.
- **Outlook (Optional)** – for future email alerts.

---

## Workflow Summary

1. **Power Automate Flow**:
   - Triggered twice daily using a recurrence trigger.
   - Fetches weather data for multiple cities using OpenWeatherMap API.
   - Parses JSON response and appends it into an Excel file stored in OneDrive.
   - Triggers Power BI to refresh the dataset.

2. **Excel File**:
   - Structured with columns for Date, City, Temperature, Humidity, and Conditions.
   - Stored in OneDrive for cloud accessibility and Power BI integration.

3. **Power BI Dashboard**:
   - Live connection to the Excel file.
   - Visuals include:
     - Filled Map for city-wise temperatures
     - Bar & Bubble charts for comparisons
     - KPI Cards for max/min/average stats
   - Conditional formatting and slicers improve interactivity.

---


## Challenges Faced
- **InsertDeleteConflict in Excel** – Resolved with clean table structures.
- **OAuth issue with email alert** – Faced issues using college email; plan to switch to Outlook.com.
- **Dataset refresh delay** – Optimized Power BI refresh timing for better performance.

---

## How to Use
1. Clone this repo:  
   `git clone https://github.com/Gangarajukonimeti2012/weather-dashboard-automation`

2. Replace the Excel file with your own and update the flow connections.

3. Import the Power BI file and update data source if needed.

4. Set up the Power Automate flow using the included `.json` export.

5. Optionally configure email notifications using Outlook or SMTP.

---

## Credits
- **OpenWeatherMap** for weather data API  
- Built using Microsoft Power Platform (Power BI & Power Automate)

---

## License
This project is for educational purposes only. Please cite appropriately if used elsewhere.
