# data-vis-project-2026
Project Proposal &amp; Dashboard for Data Visualization course
# 📊 Digital Consumption & Digital Carbon Footprint Dashboard
> **Course:** Data Visualization  
> **Repository:** https://github.com/your-username/digital-carbon-vis  

---

## 📌 1. Project Title & Background
* **Project Title:** Digital Consumption & Digital Carbon Footprint Dashboard  
* **GitHub Repository:** `https://github.com/your-username/digital-carbon-vis`  

### Background & Motivation
In the digital age, the daily use of online services—such as video streaming, cloud storage, social media platforms, and AI tools—has become an integral part of modern life. However, consumers are rarely aware that every online action consumes electricity at data centers, generating an invisible carbon footprint (**Digital Carbon Footprint**).  

**Motivation:**  
This project aims to build an interactive and multi-dimensional visualization dashboard that illustrates the relationship between individual digital consumption habits and their cumulative environmental impact over time. By translating abstract data into intuitive visual formats, this initiative seeks to raise public awareness and encourage sustainable digital consumption choices.

---

## ❓ 2. Objectives & Key Research Questions
The project addresses four core research questions:
1. **Emissions by Platform:** Which digital service categories (Streaming, Social Media, Cloud Storage, AI Tools) account for the highest carbon emissions per hour of use?
2. **Consumption Patterns:** How do digital consumption habits vary across different time slots during the day and days of the week?
3. **Correlation Analysis:** Is there a strong correlation between bandwidth consumption (GB), video/data resolution (SD, HD, 4K), and the resulting $CO_2$ emissions?
4. **Impact Projection:** If users reduce high-definition streaming by 20%, how much carbon emission would be saved, and how many trees planted does that equate to?

---

## 💾 3. Data Collection & Sources
* **Data Sources:**
  * *Secondary Data:* Open-source datasets from Kaggle, energy usage reports from the International Energy Agency (IEA), and sustainability reports published by tech companies (Google, Netflix, Meta).
  * *Primary Data:* Survey data collected from 200+ students and young adults via Google Forms regarding their daily digital service usage.
* **Collection Method:**
  * Scraping and cleaning data using Python (`requests`, `BeautifulSoup`, `pandas`).
  * Exporting survey results from Google Forms as structured `.csv` files.

---

## 🧹 4. Data Processing
* **Data Cleaning:** Handling missing values and filtering out extreme outliers in usage hours.
* **Standardization:** Converting various metrics into standardized units: Data Volume (GB), Time Duration (Hours), and Carbon Emissions ($gCO_2e$).
* **Data Transformation:** 
  * Calculating carbon emissions using the formula:  
    $$\text{Carbon Emission } (gCO_2) = \text{Data Volume (GB)} \times \text{Energy Intensity (kWh/GB)} \times \text{Grid Emission Factor}$$
  * Aggregating data across service types, time slots, and user demographics.
* **Tools Used:** Python (`pandas`, `numpy`), Google Colab / VS Code.

---

## 🎨 5. Visualization Design: 3 Draft Prototypes
1. **Prototype 1: Bar Chart & Heatmap (Emission Overview)**
   * *Description:* A Stacked Bar Chart displaying total $CO_2$ emissions by service category, combined with a Weekly Heatmap showing usage intensity across time slots.
2. **Prototype 2: Scatter Plot & Bubble Chart (Bandwidth vs. Emission Correlation)**
   * *Description:* A Scatter Plot where bubble size represents total $CO_2$ output, X-axis represents Data Volume (GB), Y-axis represents Usage Duration (Hours), and color encodes Video Resolution (SD, HD, 4K).
3. **Prototype 3: Interactive Dashboard & Sankey Diagram (Flow & Impact Conversion)**
   * *Description:* A Sankey Diagram illustrating the flow from Digital Activity $\rightarrow$ Energy Consumption $\rightarrow$ Environmental Impact ($CO_2$ equivalent converted into planted trees).

---

## 🛠️ 6. System Features

### 🔴 Must-Have Features
* **Interactive Filters:** Multi-criteria filtering by service type, time frame, and resolution.
* **KPI Summary Cards:** Key metrics showing total bandwidth used (GB), total $CO_2$ generated, and daily averages.
* **Comparative Charts:** Cross-comparison of carbon intensity across different resolutions and streaming platforms.
* **Smart Tooltips:** On-hover information displaying detailed data metrics and actionable eco-friendly tips.

### 🟡 Optional Features
* **Personal Carbon Calculator:** A user-interactive tool allowing individuals to input their daily usage hours and calculate their personal carbon footprint.
* **Scenario Simulator:** A predictive slider simulating emission reductions when downgrading video quality from 4K to Full HD.

---

## 📅 7. Project Schedule & Milestones

| Stage | Timeline | Key Tasks | Expected Deliverables |
| :--- | :--- | :--- | :--- |
| **Phase 1** | Week 1 – 2 | Data collection, cleaning, and normalization | Cleaned `.csv` dataset |
| **Phase 2** | Week 3 | Exploratory Data Analysis (EDA) & Wireframing | UI/UX Prototypes & Sketches |
| **Phase 3** | Week 4 – 5 | Dashboard development (Streamlit / Plotly / D3.js) | Alpha Dashboard Prototype |
| **Phase 4** | Week 6 | Refinement, user testing, and final documentation | Final Report & Presentation Slides |

---

## 📂 8. Repository Structure
```text
├── data/               # Raw and cleaned dataset files
│   ├── raw_data.csv
│   └── cleaned_data.csv
├── notebooks/          # Jupyter Notebooks for data preprocessing & EDA
│   └── data_cleaning.ipynb
├── src/                # Core source code for dashboard rendering
│   └── app.py
├── docs/               # Proposal sketches and documentation
│   └── proposal_sketches.pdf
├── .gitignore
├── README.md
└── requirements.txt    # Required Python libraries
