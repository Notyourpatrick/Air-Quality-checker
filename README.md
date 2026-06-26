# Live Global Air Quality Tracker Dashboard

An interactive, dark-mode web application built entirely in Python using the **Dash** framework. This dashboard connects to a live air quality data pipeline, processes real-time particulate matter ($PM_{2.5}$) metrics, and maps hazardous pollution levels globally.

## 🚀 Live Visual Preview
The application features a responsive, dual-column design optimized for analytics:
* **Left Control Panel:** Interactive threshold slider and real-time numerical metric summary cards.
* **Right Visual Workspace:** Dynamic Plotly Mapbox scatter map tracking station coordinates alongside a filterable, paginated data inventory grid.

---

## 🛠️ Tech Stack & Architecture

This project is a full-stack data application engineered entirely within the Python ecosystem:
* **Backend & Server:** Flask (via Core Dash)
* **Data Manipulation:** Pandas & NumPy
* **Data Visualization:** Plotly Express (Geospatial Mapbox)
* **Frontend UI Componentry:** React.js wrapper via Dash Core/Bootstrap Components (`dbc`)
* **Aesthetic Theme:** Cyborg Bootstrap (Dark Mode configuration)

---

## 📋 Features & Functionality

* **Live Data Ingestion:** Automatical REST API fetching via the OpenAQ API protocol.
* **Resilient Fallback Core:** Built-in geometric simulation engine that safely generates a global data array if external API servers experience rate-limits or downtime.
* **Reactive Callback Architecture:** State changes on the client-side slider automatically trigger vector filters across memory dataframes, updating all visual elements without a full page refresh.

---

## 💻 Installation & Setup

### Prerequisites
Ensure you have Python 3.8+ installed on your system.

### 1. Clone the Workspace
```bash
git clone [https://github.com/YOUR_USERNAME/air-quality-dash.git](https://github.com/YOUR_USERNAME/air-quality-dash.git)
cd air-quality-dash
