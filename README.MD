# 📊 **Energy Community Model using Calliope**

> **"Optimizing grid flexibility, renewable energy integration, and cost efficiency for energy communities in urban areas."**

---

## 📚 **Project Overview**

This repository contains the **Energy Community Model** developed as part of my **master's thesis** at **Delft University of Technology (TU Delft)** in collaboration with **Accenture**. The model uses **Calliope**, an open-source energy system modeling framework, to optimize energy distribution, reduce costs, and integrate renewable energy in urban energy systems in the Netherlands.

The thesis addresses challenges related to **grid congestion**, **energy affordability**, and **sustainability** while exploring the potential of **energy communities** to make better use of existing infrastructure.

---

## 🎯 **Objectives**

- **Optimize Grid Flexibility:** Reduce grid congestion through smarter energy distribution.  
- **Cost Efficiency:** Lower energy costs for households and stakeholders.  
- **Renewable Energy Integration:** Maximize the use of solar and battery technologies.  
- **Scalability:** Adapt the model for neighborhoods and industrial districts.  
- **Scenario Analysis:** Explore trade-offs between affordability, sustainability, and grid security.

---

## 🛠️ **Model Description**

### **Core Components**
- **Technologies:** Solar panels (PV), batteries (distributed and central), transformers, grid connections.  
- **Actors:** Distributed System Operators (DSO), Aggregators, Municipalities, Households.  
- **Scenarios:** Sensitivity scenarios addressing transformer sizes, PV capacity, energy pricing models, and battery costs.  

### **Optimization Goals**
- Minimize grid congestion.  
- Optimize energy costs.  
- Maximize renewable energy penetration.  

### **Software Tools**
- **Calliope:** Energy system optimization.  
- **Python:** Preprocessing, analysis, and visualization.  
- **Plotly:** Interactive dashboards for result visualization.

---

## 📂 **Repository Structure**

```plaintext
📁 /model_config
    ├── scenarios.yaml      # Definition of sensitivity scenarios
    ├── techs.yaml          # Technology specifications
    ├── locations.yaml      # Node and actor spatial distribution
    ├── templates.yaml      # Templates used for clarity

📁 /Experiments
    ├── 

📁 /docs
    ├── thesis.pdf          # Thesis report (final version)

📁 /data_sources
    ├── data_sources/       # Raw and preprocessed data for the model

Dashboard.ipynb     # Interactive dashboard for analysis
model.yaml          # Core Calliope model configuration
scenarios.yaml      # Core scenarios that can be used
📄 README.md        # Documentation for the project
```

---

## 🚀 **Getting Started**

### **1. Prerequisites**

Make sure you have the following tools installed:
- **Python 12.0+**
- **Calliope V7.0+**
- **Pandas**
- **Xarray**
- **Plotly**

Install dependencies using:
```bash
pip install calliope pandas xarray plotly numpy matplotlib
```

---

### **2. Model Configuration**

Adjust parameters and scenarios:
- Update **`model.yaml`** for core model settings.  
- Modify **`scenarios.yaml`** for scenario-specific configurations.

---

### **3. Run Scenarios**

- Results are saved as **NetCDF files** 

---

### **4. Analyze Results**

Generate visualizations:
- **Load Duration Curves:**
    ```bash
    python scripts/plot_duration_curves.py
    ```
- **Installed Capacity Plots:**
    ```bash
    python scripts/plot_installed_capacities.py
    ```

For interactive visualization:
- **Installed Capacity Dashboard:**
    ```bash
    python scripts/installed_capacity_dashboard.py
    ```
- **Load Duration Curve Dashboard:**
    ```bash
    python scripts/load_duration_curve_dashboard.py
    ```

---

## 📊 **Key Outputs**

- **NetCDF Files:** Scenario-specific results (`/results/sensitivity_analysis_runs`)  
- **Load Duration Curves:** Sorted time-series flows for key technologies  
- **Installed Capacity Plots:** Stacked bar charts showing capacity per technology  
- **Summary CSV:** Aggregated scenario results (`/results/all_results.csv`)

---

## 📈 **Scenario Overview**

### **Sensitivity Analysis Scenarios:**
- Transformer sizes: **undersized**, **oversized**  
- PV capacity: **undersized**, **oversized**  
- Electrification: **high**, **low**  
- Battery pricing: **medium**, **low**  
- Energy pricing: **fixed high**, **fixed low**, **mirror**

### **Objective Trade-offs:**
- **Affordability**
- **Sustainability**
- **Grid Security**

---

## 📝 **Customization**

1. **Add New Technologies:** Update `techs.yaml`.  
2. **Modify Scenarios:** Adjust parameters in `scenarios.yaml`.  
3. **Change Optimization Goals:** Update objective functions in `model.yaml`.  

---

## 🚦 **Known Limitations**

- **Network Details:** Limited visibility into low-voltage constraints.  
- **Static Scenarios:** Limited dynamic adaptation over time.  
- **Simplified Assumptions:** Some system dynamics are aggregated.

---

## 🤝 **Contributing**

Contributions are welcome!  

---

## 📬 **Contact**

**Tom de Bruin**  
**Delft University of Technology**  
**LINKEDIN:** [www.linkedin.com/in/tom-antonie-de-bruin]

---

## 🌍 **Acknowledgments**

- **Accenture Utilities Team**  
- **TU Delft Calliope Development Team**  

---

**Happy Modeling! ⚡️📊**  
**Let's optimize the energy future—together! 🌍🔋**
