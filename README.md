# Understanding Urban Transit Through Network Science

### An Analysis of Milan and Barcelona

## 📖 Project Overview

This project examines and compares the public transportation networks of **Milan** and **Barcelona**, two major European cities with extensive, multimodal transit systems. By applying **Social Network Analysis (SNA)**, we model transit stops as nodes and connections as edges to uncover structural properties, connectivity patterns, and navigational efficiencies that are often difficult to detect using traditional transport engineering approaches.

The project analyzes the efficiency, robustness, and resilience of these networks, providing insights into how they serve their respective urban populations.

## 👥 Team Members

* **Amir Masoud Aghaei** (0001165333)
* **Gita Javadi** (0001158007)
* **Omid Nejati** (0001154905)
* **Alireza Shahidiani** (0001154402)

**Course:** Artificial Intelligence  
**Date:** November 2025

## 📂 Repository Structure

* `sna_proj.ipynb`: The main Jupyter Notebook containing the data extraction, graph construction, analysis, and visualization code.
* `SNA Report.pdf`: The final report detailing the methodology, results, mathematical background, and conclusions.

## 🛠️ Technologies & Libraries

The analysis is performed using Python. The primary libraries used include:

* **NetworkX:** For graph creation and calculation of network metrics (centrality, degree distribution, etc.).
* **OSMnx & Folium:** For geospatial visualization and mapping.
* **Pandas & NumPy:** For data manipulation.
* **GTFS Kit:** For processing General Transit Feed Specification data.
* **Matplotlib & Seaborn:** For statistical plotting.

## 🚀 Getting Started

To run the analysis code on your local machine or Google Colab, follow these steps:

### Prerequisites

Ensure you have Python installed. You will need to install the required dependencies.

### Installation

If you are running this locally, it is recommended to create a virtual environment first. Then, install the required packages using the command below (derived from the notebook configuration):

```bash
pip install osmnx folium networkx matplotlib numpy pandas geopandas shapely tqdm gtfs_kit pyproj contextily seaborn scikit-learn
````

### Running the Analysis

1.  Clone this repository.
2.  Open `sna_proj.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
3.  Ensure your dataset (GTFS files) is placed in the correct directory as referenced in the notebook (or update the file paths in the code).
4.  Run all cells to generate the graphs and statistics.

## 📊 Methodology

The project follows these main analytical steps:

1.  **Data Ingestion:** Loading GTFS data (stops, routes, trips) for Milan and Barcelona.
2.  **Graph Construction:**
      * **Nodes:** Public transport stops.
      * **Edges:** Direct connections between stops via transit lines.
3.  **Topological Analysis:** Calculating metrics such as:
      * Degree Distribution
      * Clustering Coefficient
      * Average Path Length
      * Betweenness & Closeness Centrality
4.  **Resilience Testing:** Simulating node failures (random vs. targeted attacks) to see how the network connectivity degrades.

## 🔗 Data Sources

  * **Milan:** [Azienda Trasporti Milanesi (ATM)](https://www.atm.it/)
  * **Barcelona:** [Transports Metropolitans de Barcelona (TMB)](https://www.tmb.cat/)
  * **Aggregators:** [Transitland](https://www.transit.land/) & [GTFS.org](https://gtfs.org/)

## 📄 License

This project is created for academic purposes. Please refer to the `SNA Report.pdf` for full citations and references.
