# 🚕 Uber Trip Analysis - Power BI Dashboard

This project presents an end-to-end data analytics solution using **Power BI** to analyze Uber trip data. It offers interactive dashboards to uncover booking patterns, revenue insights, trip efficiency, location trends, and time-based demand. The objective is to support data-driven decisions across business units.

---

## 📊 Dashboards Overview

### 🧩 Dashboard 1: Overview Analysis

**Purpose:** Analyze booking trends, revenue generation, and trip efficiency.

#### 🔑 KPIs:
- **Total Bookings** – Total number of trips.
- **Total Booking Value** – Total revenue from trips.
- **Average Booking Value** – Average revenue per booking.
- **Total Trip Distance** – Total distance traveled.
- **Average Trip Distance** – Average distance per trip.
- **Average Trip Time** – Average duration per trip.

#### 📈 Visuals:
- **Measure Selector** (Disconnected Table):
  - Select from `Total Bookings`, `Total Booking Value`, `Total Trip Distance` to dynamically update visuals.
- **By Payment Type**: Chart split by Card, Cash, Wallet, etc.
- **By Trip Type**: Day vs Night.
- **Vehicle Type Grid View**:
  - Table/Matrix with KPIs across different vehicle types.
  - Conditional formatting and sorting enabled.
- **Total Bookings by Day**: Detect peak and off-peak trends.

#### 🌍 Location Analysis:
- **Most Frequent Pickup Points**
- **Most Frequent Drop-off Points** *(requires inactive relationship activation)*
- **Farthest Trip** based on distance
- **Top 5 Booking Locations**
- **Most Preferred Vehicle per Pickup Location**

#### 💡 Additional Enhancements:
- Dynamic Title for charts based on selected measure.
- Interactive **Slicers**: Date, City, Trip Type, Vehicle Type.
- Tooltips with extra KPIs like Avg Trip Distance or Booking Value.
- **Bookmark**: "Data Details" – explaining metrics, tables used, source info.
- **Clear Slicer Button**: One-click reset of all filters.
- **Download Raw Data Button**: Export data to Excel/CSV via Power Automate or native export.

---

### ⏰ Dashboard 2: Time Analysis

**Purpose:** Analyze trip demand based on time for operations and pricing optimization.

#### 🔄 Global Dynamic Measure:
Updates all visuals based on user selection:
- Total Bookings
- Total Booking Value
- Total Trip Distance

#### 📊 Visuals:
- **Area Chart**: Bookings by Pickup Time (grouped in 10-minute intervals)
- **Line Chart**: Booking patterns by Day Name (Mon–Sun)
- **Heatmap (Matrix Grid)**:
  - **Rows**: Hours of the day (0–23)
  - **Columns**: Days of the week (Mon–Sun)
  - **Values**: Selected dynamic measure
  - Highlights peak hours and days

---

### 🧾 Dashboard 3: Details Tab

**Purpose:** Provide detailed trip-level data and enable drill-through exploration.

#### Features:
- **Grid Table**: Key trip fields like Trip ID, Date, Time, City, Payment Type, Vehicle Type, Distance, Duration.
- **Drill-through**: From charts/heatmaps to this detailed tab.
- **Bookmark**: “View Full Data” – toggle between filtered and all records.

---

## 🧠 Business Objectives

✔ Identify trends in ride bookings and revenue generation  
✔ Analyze trip efficiency in terms of distance and duration  
✔ Compare trip patterns by vehicle type, location, and time  
✔ Enable pricing optimization and operational planning  
✔ Provide transparency with raw data access and drill-down views

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **Power Query (M Language)**
- **DAX (Data Analysis Expressions)**
- **Power Automate** (optional, for export functionality)
- **Bookmarks, Buttons, Tooltips, Slicers, Drill-throughs**

This project is licensed under the [Apache 2.0](LICENSE)

