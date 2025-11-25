# 📊 Population Analysis Dashboard – Power BI

A complete analytical Power BI project visualizing **Male & Female Population**, **regional distributions**, **country-level insights**, and **age categories** from multiple years. This dashboard provides interactive slicers, charts, and KPIs to understand demographic patterns effectively.

---

## 🚀 Project Overview

This Power BI report focuses on visualizing global population data categorized by:

- 🔹 Male Population  
- 🔹 Female Population  
- 🔹 Total Population  
- 🔹 Region-wise distribution  
- 🔹 Country-wise population values  
- 🔹 Age Categories (Baby, Small Kid, Teenager, Young, Senior, etc.)  
- 🔹 Year selection (1950–2001)  

The dashboard contains multiple visuals such as pie charts, bar charts, funnel charts, and gauges to explore population changes across regions and timelines.

---

## 🖼 Dashboard Preview

### **Dashboard 1 – Population by Gender**
![Dashboard 1](./image/1.jpg)

### **Dashboard 2 – Total Population Insights**
![Dashboard 2](./image/2.png)

_Add your image files inside `/assets` folder_

---

## 📂 Features Included

### ✔ **KPI Cards**
- Total Population  
- Male Population  
- Female Population  
- Region-wise totals  

### ✔ **Charts Used**
- Donut Charts (Region distribution)  
- Bar Charts (Population by region)  
- Funnel Chart (Female population breakdown)  
- Gauge Chart (Male population insights)  
- Pie Chart (Country population share)  

### ✔ **Filters & Slicers**
- Year (1950 – 2001)  
- Gender (Male / Female)  
- Age Category  

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard Creation |
| **Excel / CSV Dataset** | Data Input |
| **DAX** | Measures & Calculations |
| **Power Query** | Data Cleaning |

---

## 📘 Key DAX Measures

```DAX
Total Population = SUM(Population[Value])

Male Population = 
    CALCULATE(
        SUM(Population[Value]), 
        Population[Gender] = "Male"
    )

Female Population = 
    CALCULATE(
        SUM(Population[Value]), 
        Population[Gender] = "Female"
    )
