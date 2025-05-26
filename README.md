
# 🚚 Shipping Optimization Project

This project focuses on optimizing shipping routes between multiple US cities using real-world data and big data simulation. It leverages Google Maps Distance Matrix, Weather APIs, and generates large-scale shipping data (~20GB) to analyze, optimize, and visualize efficient delivery paths.

---

## 📖 Table of Contents
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Project Structure](#project-structure)
- [Summary](#summary)
- [How to Run](#how-to-run)
- [Key Features](#key-features)
- [Contributors](#contributors)
- [License](#license)

---

## 🔧 Prerequisites
- Python 3.x
- Jupyter Notebook
- Apache Hadoop & Spark (with Java, Python, PySpark)
- Install required Python libraries:
```bash
pip install pandas numpy requests matplotlib seaborn folium googlemaps
```

---

## 🗂 Project Structure
```
📁 Shipping-Optimization/
├── Book1.ipynb  # Data Generation: Google API, Weather API, and 20GB shipping data
├── Book2.ipynb  # Data Analysis: EDA, Optimizations on Distance Matrix
├── Book3.ipynb  # Advanced Analysis: Weather Impact, Algorithm Comparisons
├── data/
│   └── real_distance_matrix.csv  # Distance matrix from Google API
├── output/
│   └── generated_data/      # Folder for generated shipping data
├── visualizations/
│   └── tsp_route_map.html   # Interactive TSP route map
│   └── ga_route_map.html    # Genetic Algorithm route map
├── .gitignore               # Exclude data files, outputs
├── LICENSE                  # MIT License
└── README.md                # Project documentation
```

---

## 📈 Summary
1. **Fetch Real Data**: Uses Google Maps API and Weather API to generate a real-world distance matrix.
2. **Generate Big Data**: Creates a large (~20GB) shipping dataset with added weather and traffic impact.
3. **Analyze & Optimize**: Performs EDA, visualizes data, and applies various optimization algorithms (Greedy TSP, Genetic Algorithm, Christofides, etc.).
4. **Weather & Traffic Considerations**: Adjusts routes based on real-time data.
5. **Final Route Solution**: Identifies the optimal delivery path using real-time adjusted distances.

---

## 🚀 How to Run
1️⃣ **Clone the repository:**
```bash
git clone https://github.com/yourusername/shipping-optimization.git
cd shipping-optimization
```

2️⃣ **Ensure Apache Hadoop & Spark are installed and configured.**

3️⃣ **Run notebooks in order:**
- **Book1.ipynb**: Generate distance matrix & big data.
- **Book2.ipynb**: Analyze data, visualize, optimize.
- **Book3.ipynb**: Add weather impact, compare algorithms, finalize route.

4️⃣ **View results**: Explore interactive maps, charts, and optimal routes in `/visualizations`.

---

## ✨ Key Features
- 📍 Real-time data fetching from Google Maps and Weather APIs.
- 📦 Large-scale (~20GB) synthetic shipping data generation.
- 📊 In-depth EDA and visualization of shipping trends.
- 🧠 Multiple optimization algorithms:
  - Greedy TSP
  - Genetic Algorithm (GA)
  - Christofides
  - Asadpour ATSP (advanced)
- 🌦 Weather and traffic impact on routes.
- 🗺 Interactive map visualizations using Folium and Plotly.
- 💻 Scalable analysis with Apache Hadoop & Spark.

---

## 👥 Contributors
- **[Your Name]** – Data Engineer & Optimization Specialist  
- **[Team Member 2]** – Visualization & Data Analysis  
- **[Team Member 3]** – Weather & Traffic Data Integration

---

## 📚 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
