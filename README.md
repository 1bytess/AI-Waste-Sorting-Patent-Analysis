# AI-Based Automated Waste Sorting System: Patent Landscape Analysis

## 📖 Overview

This project presents a comprehensive analysis of patents related to AI-based automated waste and recycling sorting systems. The primary goal is to understand the current technology landscape, identify key players, analyze technological trends, and discover opportunities for innovation. By analyzing patent data, we can identify core technologies, assess the potential for patent infringement, and propose novel ideas for future development.

This analysis was conducted as part of the "Big Data Case Studies" course.

---

## 📂 Project Structure

The repository is organized as follows:
```
.
├── data/                  
│   ├── xlsx/
│   ├── korean_patents_automatic_sorting_500.csv
│   ├── korean_patents_B07C5_34_500.csv
│   ├── korean_patents_computer_vision_500.csv
│   ├── korean_patents_G06V10_00_16.csv
│   └── korean_patents_recyclable_materials_500.csv
│├── export/              
│   ├── analysis_summary.csv
│   ├── cleaned_patent_data.csv
│   └── core_patents.csv
│├── plot/                
│   ├── analysis_notebook_21_0.png
│   ├── analysis_notebook_22_0.png
│   ├── analysis_notebook_23_0.png
│   ├── analysis_notebook_24_0.png
│   ├── analysis_notebook_25_0.png
│   ├── analysis_notebook_26_0.png
│   └── tech_network.png
│├── report/               
│   └── 기말_빅데이터사례연구_2021012800_벤네딕터스 에스라 헤르노오.pdf
├── analysis_notebook.ipynb 
├── requirements.txt      
└── README.md                    
```
---

## 📊 Dataset

The patent data was collected from Korean patent databases using specific keywords and IPC (International Patent Classification) codes relevant to automated sorting and computer vision technology.

* **Keywords:** "자동 분류" (automatic sorting), "컴퓨터 비전" (computer vision), "재활용품" (recyclables)
* **IPC Codes:**
    * `B07C 5/34`: Separating solid materials using electronic or photoelectric means
    * `G06V 10/00`: Image or video recognition or understanding
* **Data Files:** The `data/` directory contains the raw CSV files downloaded for each search query. Each file represents a set of up to 500 patents matching the criteria.

---

## 🔬 Analysis

The core of the analysis is documented in the `analysis_notebook.ipynb` Jupyter Notebook. The key steps include:

1.  **Data Loading & Preprocessing:** Loading the raw CSV files, merging them, and cleaning the data (e.g., handling duplicates, parsing dates, standardizing text). The cleaned dataset is saved in `export/cleaned_patent_data.csv`.
2.  **Quantitative Analysis:**
    * **Trend Analysis:** Examining the number of patent applications over the years to identify growth and peak periods.
    * **Applicant Analysis:** Identifying the top applicants (companies, institutions, individuals) to understand the key players in the field.
    * **Technology Hotspots:** Analyzing the frequency of specific IPC codes to map the core technological areas.
3.  **Qualitative Analysis:**
    * **Core Patent Deep Dive:** An in-depth analysis of selected core patents to understand their technological claims, scope of rights, and potential for avoidance design.
    * **Technology Network Visualization:** Creating a network graph (`plot/tech_network.png`) to visualize the relationships between different technologies and applicants.

The plots generated during the analysis are saved in the `plot/` directory.

---

## ✨ Results & Key Findings

The analysis revealed several key insights:

* **Market Growth:** A significant increase in patent filings was observed, peaking around 2021, indicating a surge in R&D in this domain.
* **Key Technologies:** Computer vision (`G06V`) and specific sorting mechanisms (`B07C`) are central to the patented technologies.
* **Innovation Opportunity:** The analysis identified a gap in the market for systems that use multi-sensor fusion (e.g., combining vision, spectral, and weight sensors) and edge AI processing for faster, more accurate, and scalable sorting. This led to the proposal of a novel "Multi-Sensor Fusion AI Recycling Sorting System".

The final project report, `report/기말_빅데이터사례연구_....pdf`, contains a detailed explanation of the methodology, findings, and strategic recommendations.

---

## 🚀 How to Run

To reproduce this analysis, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/AI-Waste-Sorting-Patent-Analysis.git](https://github.com/your-username/AI-Waste-Sorting-Patent-Analysis.git)
    cd AI-Waste-Sorting-Patent-Analysis
    ```

2.  **Set up the Python environment:**
    It is recommended to use a virtual environment.
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Jupyter Notebook:**
    Launch Jupyter and open the `analysis_notebook.ipynb` file.
    ```bash
    jupyter notebook
    ```
    You can then run the cells in the notebook to execute the entire analysis pipeline.

---
## 📝 Dependencies
This project relies on common Python libraries for data science, which are listed in `requirements.txt`. Key dependencies include:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `jupyter`
