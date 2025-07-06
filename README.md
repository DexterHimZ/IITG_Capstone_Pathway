# IITG_Capstone_Pathway
# Dynamic Pricing for Urban Parking Lots

### 🚀 Capstone Project – Summer Analytics 2025

This project implements a real-time, data-driven pricing engine for urban parking lots using only Python, Pandas, NumPy, and Pathway. The objective is to dynamically adjust parking prices based on demand, competition, and real-time conditions across 14 parking locations.

---

## 📂 Project Structure

* `Model 1 – Baseline Linear Model`: Price increases linearly with occupancy.
* `Model 2 – Demand-Based Pricing`: Embedded in UDF logic; combines dynamic city features.
* `Model 3 – Competitive Pricing Model`: Incorporates geographic proximity and competitor prices to adjust pricing.
* `Dynamic Features`: Traffic, queue length, special days, vehicle types.
* `Geospatial Logic`: Computes distance between lots.
* `Visualization`: Static price trend comparison using Bokeh.

---

## 🛠️ Technologies Used

* **Python**: Core implementation
* **Pandas & NumPy**: Data manipulation and computation
* **Pathway**: Real-time logic via `@pw.udf`
* **Bokeh**: Interactive pricing visualizations

---

## 📈 How Pricing Works

* Starts with a base price of \$10
* Adjusts based on:

  * Occupancy rate
  * Queue length
  * Nearby traffic congestion
  * Special events or holidays
  * Type of incoming vehicle
  * Competitor proximity and pricing

---

## 📊 Visualization

Bokeh line plots track pricing across all models for each parking lot. These help visualize how different models respond to demand.

---

## ✅ Implemented Models

| Model   | Description                               | Implemented            |
| ------- | ----------------------------------------- | ---------------------- |
| Model 1 | Linear price w\.r.t occupancy             | Yes                    |
| Model 2 | Demand-based pricing                      | Yes (within UDF logic) |
| Model 3 | Competitive pricing with geospatial logic | Yes                    |

---

## 🧠 Architecture

1. **Data Ingestion**: 73-day simulation over 14 lots with time-stamped intervals.
2. **Feature Extraction**: Parse occupancy, traffic, vehicle types, etc.
3. **Pricing Logic**:

   * Model 1: Linear Occupancy
   * Model 2: Demand Score via city & vehicle factors
   * Model 3: Adjust with competitor prices and distance
4. **Real-Time Processing**:

   * Pathway UDF for model execution
5. **Visualization**:

   * Bokeh pricing plots

---

## 📜 License

This project is part of Summer Analytics 2025, hosted by Consulting & Analytics Club × Pathway.

---

## 👤 Author

HIMANGSHU SHEKHAR
