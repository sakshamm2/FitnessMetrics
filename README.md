# 🏋️ Gym Performance Dashboard — Power BI

An executive-level **Gym Performance Dashboard** built in Microsoft Power BI to provide a consolidated view of gym revenue, membership activity, attendance, acquisition channels, branch performance, and trainer analytics.

The dashboard transforms operational gym data into actionable business insights through an interactive, clean, and portfolio-ready BI experience.

---

## 📊 Dashboard Overview

The Gym Performance Dashboard provides a centralized view of key business and operational metrics.

### Key Performance Indicators

| KPI                      |         Value |
| ------------------------ | ------------: |
| 💰 Total Revenue         |      **$7M+** |
| 👥 Active Members        |       **218** |
| 🏃 Total Attendance      |       **15K** |
| ⏱️ Avg. Session Duration | **72.7 mins** |

---

## 🎯 Project Objectives

The dashboard was designed to answer key business questions such as:

* How is gym revenue performing over time?
* Which branches generate the most revenue?
* How many members are currently active?
* What is the overall attendance volume?
* Which membership statuses dominate the customer base?
* Which channels acquire the most members?
* What workout types are most popular?
* Which trainers have the highest average session durations?

The goal was to turn raw operational data into a **single, interactive source of truth for management decision-making**.

---

## 🚀 Key Features

### 💰 Revenue Analysis

* Total Revenue KPI
* Monthly revenue trend analysis
* 2024–2025 revenue performance
* Branch-level revenue comparison
* Interactive date filtering

### 👥 Membership Analytics

* Active member tracking
* Membership status distribution
* Expired, Active, and Cancelled member analysis
* Member acquisition channel analysis

### 🏃 Attendance & Workout Analytics

* Total attendance tracking
* Workout type preference analysis
* Attendance breakdown by workout category
* Average session duration

### 🏢 Branch Performance

* Revenue comparison across IronCore branches
* Branch-level performance analysis
* Interactive cross-filtering between branches and other dashboard metrics

### 🧑‍🏫 Trainer Analytics

* Trainers ranked by session duration
* Comparative trainer performance
* Interactive filtering

---

## 🧱 Data Architecture

The dashboard uses a **relational star-schema data model** designed to support scalable analytics and efficient cross-filtering.

### Core Tables

```text
                    ┌─────────────────┐
                    │   tblCalendar   │
                    └────────┬────────┘
                             │
                             ▼
┌──────────────┐      ┌───────────────┐      ┌──────────────┐
│ tblMembers   │─────▶│ tblMemberships│◀─────│   tblPlans   │
└──────────────┘      └───────────────┘      └──────────────┘
        │
        ▼
┌────────────────┐
│ tblAttendance  │
└───────┬────────┘
        │
        ▼
┌────────────────┐
│  tblTrainers   │
└────────────────┘

┌────────────────┐
│  tblPayments   │
└───────┬────────┘
        │
        ▼
┌────────────────┐
│  tblBranches   │
└────────────────┘
```

### Tables Used

* `tblMembers`
* `tblMemberships`
* `tblPayments`
* `tblAttendance`
* `tblBranches`
* `tblTrainers`
* `tblPlans`
* `tblCalendar`

The model uses established relationships and a dedicated calendar table to support reliable time-based analysis and chronological reporting.

---

## 🔄 Interactive Analytics

The dashboard uses Power BI's relational model and cross-filtering capabilities to allow users to explore the data dynamically.

For example:

**Branch → Revenue → Members → Attendance → Trainer Analytics**

Selecting a relevant dimension updates connected visuals throughout the report.

---

## 🎨 UI/UX Design

The dashboard follows a minimalist executive BI design philosophy.

### Design Principles

* Clean light-mode interface
* Dark navy/slate visual elements
* White card containers
* Subtle borders
* Consistent typography
* Clear KPI hierarchy
* Structured visual spacing
* Concise chart titles
* Optimized axis labels
* Minimal visual clutter

The objective was to make the dashboard both **analytically useful and presentation-ready**.

---

## 🛠️ Tools & Technologies

* **Microsoft Power BI**
* **Power Query**
* **DAX**
* **Excel**
* Relational data modeling
* Star-schema architecture
* Interactive dashboard design

---

## 📈 Business Insights

The dashboard provides visibility into several important business dimensions:

### Revenue

Revenue exceeded **$7M**, with monthly trends providing visibility into changes across 2024–2025.

### Membership

The dashboard provides a clear view of the relationship between active, expired, and cancelled memberships.

### Acquisition

Member acquisition channels can be compared to identify the channels contributing the highest number of members.

### Attendance

With approximately **15K attendance records**, the dashboard provides visibility into member engagement and workout preferences.

### Trainer Performance

Trainer analytics rank trainers according to session duration, helping identify differences in member engagement and session activity.

---

## 📂 Project Structure

```text
Gym-Performance-Dashboard/
│
├── README.md
│
├── Gym_Performance_Dashboard.pbix
│
├── Dataset/
│   └── gym_dataset.xlsx
│
└── Screenshots/
    └── dashboard.png
```

> File names may vary depending on the final repository structure.

---

## ▶️ How to View the Dashboard

### Option 1 — Power BI Desktop

1. Download the `.pbix` file from this repository.
2. Install **Microsoft Power BI Desktop** if it is not already installed.
3. Open the `.pbix` file.
4. If Power BI asks for a data-source path, update the source to the included dataset.
5. Refresh the data if required.
6. Interact with the dashboard using the available slicers and visual filters.

### Option 2 — Dashboard Screenshot

A preview of the completed dashboard is available below.

![Gym Performance Dashboard](dashboard.png)

---

## 📌 Portfolio Highlights

This project demonstrates practical experience with:

* Data modeling
* Star-schema architecture
* Power Query data preparation
* DAX measures
* Time-series analysis
* KPI development
* Interactive filtering
* Business intelligence visualization
* Dashboard UI/UX design
* Business insight generation

---

## 👤 Author

**Saksham Yadav**

B.Tech — Computer Science

This project was created as part of my portfolio to demonstrate practical **Power BI, data analytics, and business intelligence** capabilities.
