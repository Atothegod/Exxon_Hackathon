# ExxonMobil Hackathon 2025

## Challenge Overview
This project was developed as part of the **ExxonMobil Hackathon 2025** under the theme: **Analytics & Innovation for Sustainable Operations**.

---

## Business Context

### Organization Overview
- **Parent Company**: Exxon Mobil Corporation, USA – Over 140 years in global energy, gas, and petroleum.
- **Vision**: *Leader of innovation advancing modern living.*
- **Purpose**: *Sustainably improve quality of life.*
- **Key Divisions**:
  - Upstream (e.g., deep-sea drilling, LNG)
  - Product Solutions (e.g., fuel, chemical, lubricants)
  - Low Carbon Solutions (e.g., CCS, biofuels, lithium for EVs)

---

## Business Case: Polymer Product Logistics

The core problem involves warehouse **inventory imbalance**, where mismatch between **inbound shipments** (based on 3-month demand planning) and **outbound logistics** (truck/marine) causes:
- Overflow costs (D&D)
- Understock scenarios
- Inefficient space utilization

**Warehouse KPIs**:
- Maximize utilization without breaching capacity
- Maintain inventory levels in optimal range (target: 70–80% capacity)
- Predict and adjust future stock fluctuations early

---

## Dataset Description

The dataset used includes:
- `Warehouse_Max_Capacity`
- `On_Ground_Inventory_2024`
- `Inbound_Data`
- `Outbound_Data`
- `Forecasted_Demand & Sales`
- `Material_Master_Data`

---

## Solution Approach

### 1. Descriptive Analytics (EDA & Monitoring)

- Cleaned and standardized all data sources
- Created inventory monitoring dashboard
- Built **Overflow Risk Alerts**
- Visualized historical trends of inventory, inbound, outbound movement

### 2. Forecast Adjustment

> *We performed forecast adjustment using historical accuracy deviation, resulting in significantly improved alignment between actual vs predicted inventory movements.*

- Applied statistical corrections to initial forecast

---

### 3. Optimization Engine

#### Phase 1 – Historical Simulation Model

- Developed an optimization model using past data (Jan–Sept 2024)
- Objective: Avoid overflow, minimize understock, balance warehouse utilization
- Constraints: Warehouse capacity, inbound/outbound schedule, demand window

#### Phase 2 – **Predictive Optimization with Forecasted Data**

>  **Build a New Optimization Function for `pred_data`**  
> **Constructed a second optimization function using the same logic, now operating on `pred_data` (forecasted inventory & outbound trends).**

- Plug-and-play design allows users to **directly use new forecast data**
- Optimizer recommends ideal monthly in/out scheduling
- Output shows stable inventory around 70–80% with reduced overflow risk

 *This step ensures scalability and adaptability.*

---

## Technical Stack

- **Python** (Pandas, Numpy, Matplotlib, Scikit-learn, pulp)
- **Jupyter Notebook** for modeling
- **Version Control**: Git & GitHub

---

## Highlights & Innovation Value

| Area | Innovation |
|------|------------|
| Forecast Refinement | Enhanced accuracy using post-forecast adjustments |
| Optimization | Scalable predictive optimizer on clean forecast data |
| Decision Support | Actionable monthly output for warehouse planning |

> The final solution achieved stable performance and adaptability, supportSng **decision-making before shipment occurs**, aligned with **ExxonMobil's sustainability and efficiency mission.**

---

## Hackathon Criteria Mapping

| Criteria | Our Approach |
|----------|--------------|
| Innovation & Creativity | Forecast-adjusted optimizer with alert system |
| Technical Implementation | Custom EDA + Optimization engine |
| Impact & Scalability | Reduced overflow; scalable for new demand |
| Presentation & Insight | Clear narrative, action-ready dashboard |

---

## Q&A Ready

Feel free to reach out with any questions or review the notebooks for step-by-step logic explanation and model decisions.

>  *Innovation isn’t just solving a problem, but making the solution reliable, extensible, and sustainable at scale.*

---

