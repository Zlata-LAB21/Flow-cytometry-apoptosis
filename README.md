```markdown
# Flow Cytometry Analysis & Visualization Tool

An adaptive, interactive Jupyter Notebook pipeline designed for automated processing of FCS files. While specifically developed for **Apoptosis Analysis** (Annexin V / PI), the tool's architecture is flexible enough for any dual-channel flow cytometry data.

## 🔬 Core Purpose
This tool was developed to simplify the transition from raw data to publication-ready figures. It automates the heavy lifting of data scaling and population counting while keeping the researcher in control of the gating logic.

## ✨ Key Features
* **Flexible Channel Selection:** You don't need to hard-code your channels. The tool scans your FCS headers and lets you **select target channels dynamically** during execution.
* **Universal Application:** Ideal for Apoptosis (FITC/PI), but can be used for Cell Cycle, Transfection efficiency, or any experiment requiring scatter plots and quadrant gating.
* **Smart Visualization:** * Automatically generates density/scatter plots with proper dimensions.
    * Real-time quadrant analysis with live percentage updates.
    * Adaptive axis scaling based on data distribution (99.9th percentile).
* **Interactive Gating:** Set your debris gates and quadrant thresholds using intuitive input prompts.

## 📊 Output Examples
The pipeline generates high-resolution plots featuring:
1. **FSC vs SSC:** For initial cell population isolation.
2. **Fluorescence Scatter Plots:** With overlayed quadrant gates (e.g., Q1: Necrotic, Q2: Late Apoptotic, Q3: Live, Q4: Early Apoptotic).
3. **Statistical Tables:** Percentage distribution for each quadrant.

## 🛠 Installation & Setup
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Zlata-LAB21/Flow-cytometry-apoptosis.git](https://github.com/Zlata-LAB21/Flow-cytometry-apoptosis.git)

```

2. **Install dependencies:**
```bash
pip install -r requirements.txt

```

## 🚀 Workflow

1. **Data:** Place your `.fcs` files in a `fcs.zip` archive.
2. **Run:** Execute the notebook cells in order.
3. **Select:** When prompted, choose your fluorescence channels from the provided list.
4. **Adjust:** Enter your gate coordinates to see the quadrants update automatically on the plots.

## 📦 Dependencies

* `fcsparser`, `pandas`, `matplotlib`, `seaborn`, `numpy`.

---

*Developed for research purposes at IBPPM (ИБФРМ РАН).*
```
