# ⚡ Electric Vehicle (EV) Charging Infrastructure Analysis - Germany


A data-driven analysis and visualization project exploring the distribution, density, and operator dominance of Electric Vehicle (EV) charging stations across Germany, with a focused case study on the city of **Amberg**.

---

## 📑 Table of Contents

- [📍 Project Overview](#-project-overview)
- [🎯 Objectives](#-objectives)
- [🗂️ Dataset](#-dataset)
- [🛠️ Technologies Used](#-technologies-used)
- [📂 Project Structure](#-project-structure)
- [🚀 Installation & Setup](#-installation--setup)
- [📊 Analysis & Workflow](#-analysis--workflow)
- [📌 Key Insights](#-key-insights)
- [🧑‍💻 Author](#-author)
- [📜 License](#-license)

---

## 📍 Project Overview

With the rapid adoption of electric vehicles, robust charging infrastructure is critical. This project leverages Python to analyze the **Bundesnetzagentur** dataset, identifying regional disparities and infrastructure density.

The analysis covers:
* **State-level distribution** (Bundesländer)
* **City-level rankings** (excluding major metros)
* **Operator market share**
* **Geospatial visualization** (Interactive & Static maps)
* **Case Study:** Deep dive into Amberg's EV infrastructure.

---

## 🎯 Objectives

* **Analyze** the distribution of charging stations across all 16 German states.
* **Identify** regional extremes (highest vs. lowest density).
* **Discover** top-performing medium-sized cities (excluding Berlin, Munich, Hamburg, Cologne).
* **Case Study:** Analyze **Amberg** for total stations, power output, and location mapping.
* **Determine** the top 5 dominant charging station operators.
* **Visualize** data using Bar Charts, Choropleth Maps, and Folium Interactive Maps.

---

## 🗂️ Dataset

The analysis is based on the following dataset:

* **File Name:** `ev_charging_germany.csv`
* **Source:** Public EV infrastructure data (e.g., Bundesnetzagentur).
* **Format:** CSV (Semicolon `;` separated)
* **Encoding:** UTF-8

### 🗝️ Key Variables

| Column Name | Description |
| :--- | :--- |
| `Bundesland` | German State (e.g., Bayern, Berlin) |
| `Ort` | City / Municipality |
| `Betreiber` | Charging Station Operator |
| `AnzahlLadepunkteNLL` | Number of Charging Points per Station |
| `InstallierteLadeleistungNLL` | Installed Charging Power (kW) |
| `Breitengrad` | Latitude (Geospatial) |
| `Laengengrad` | Longitude (Geospatial) |

---

## 🛠️ Technologies Used

The project is built using **Python 3.x** and the following libraries:

* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Geospatial Analysis:** `geopandas`, `folium`

---

## 📂 Project Structure

```text
ev-charging-analysis/
│
├── data/
│   └── ev_charging_germany.csv    # Raw dataset (Input)
│
├── notebooks/
│   └── analysis.ipynb             # Jupyter Notebook with full code
│
├── images/                        # Generated plots and maps
│   ├── stations_by_state.png
│   └── amberg_map.html
│
├── README.md                      # Project Documentation
└── requirements.txt               # Python dependencies
🚀 Installation & Setup
Follow these steps to run the project locally:

1. Clone the Repository
Bash

git clone [https://github.com/your-username/ev-charging-germany.git](https://github.com/your-username/ev-charging-germany.git)
cd ev-charging-germany
2. Install Dependencies
Ensure you have Python installed. Then run:

Bash

pip install pandas numpy matplotlib seaborn geopandas folium
3. Run the Analysis
You can run the analysis via a Python script or Jupyter Notebook:

Bash

jupyter notebook notebooks/analysis.ipynb
📊 Analysis & Workflow
The project follows a structured data science pipeline:

1️⃣ Data Loading & Cleaning
Reading CSV with specific encodings.

Handling missing values and data types.

2️⃣ State-Level Analysis
Metric: Total charging stations per state.

Visual: Horizontal Bar Chart.

Outcome: Ranking of states (e.g., Bavaria vs. Bremen).

3️⃣ Geospatial Mapping
Method: Merging data with GeoJSON of German states.

Visual: Choropleth Map (Darker shade = Higher density).

4️⃣ City-Level & Case Study (Amberg)
Filtering: Removing top 4 major metros to find hidden leaders.

Amberg Deep Dive:

Total Stations & Power Calculation.

Visual: Interactive Folium Map marking specific coordinates in Amberg.

5️⃣ Operator Analysis
Metric: Market share by number of charging points.

Visual: Bar chart of the Top 5 Operators.

📌 Key Insights
💡 Regional Disparity: Western and Southern states (e.g., Bavaria, NRW) show significantly higher infrastructure density than Eastern states.

💡 Hidden Gems: Several medium-sized cities outperform larger counterparts when normalized for population.

💡 Amberg Case Study: Amberg demonstrates a well-distributed network relative to its urban area.

💡 Market Concentration: The top 5 operators control a substantial portion of the public charging network.

🧑‍💻 Author
Alla Sai Surya

MSc AI for Industrial Applications

📍 Germany 🇩🇪

If you have any questions or feedback, feel free to reach out!

📜 License
This project is licensed under the MIT License - see the LICENSE file for details. Intended for academic and educational purposes.
