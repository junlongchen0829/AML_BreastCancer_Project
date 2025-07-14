# Breast Cancer Classification Project

This project implements a machine learning pipeline to classify breast cancer tumors (malignant or benign) using the Breast Cancer Wisconsin (Diagnostic) dataset. The project also includes model interpretability analysis using SHAP values to explain the predictions.

---

## Dataset

- **Name**: Breast Cancer Wisconsin (Diagnostic) Data Set  
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
- **Files used**:
  - `wdbc.data`: dataset containing 569 samples and 30 features
  - `wdbc.names`: feature description

---

## Project Structure

\`\`\`
📂 breast-cancer-wisconsin-diagnostic/
├── 01_linear_classifier_pipeline.ipynb
├── 02_interpretability_shap.ipynb
├── 02_interpretability_shap_fixed.ipynb
├── AML_project_SHAP_clean_final.ipynb
├── random_forest_model.pkl
├── SHAP_Report.pdf
├── untitled.md
├── wdbc.data
├── wdbc.names
└── README.md  ← You are here!
\`\`\`

---

## How to Run

1. Clone this repo or download the folder.
2. Create a conda environment and install required packages:
    \`\`\`bash
    conda create -n bc-env python=3.10
    conda activate bc-env
    pip install -r requirements.txt  # if requirements.txt is provided
    \`\`\`
3. Open the notebook:
    \`\`\`bash
    jupyter notebook
    \`\`\`
4. Run the notebooks in order:
    - `01_linear_classifier_pipeline.ipynb`
    - `02_interpretability_shap.ipynb`

5. Export Markdown Report to PDF:
    \`\`\`bash
    pandoc untitled.md -o SHAP_Report.pdf --from markdown --pdf-engine=xelatex
    \`\`\`

---

## Results

The best model is **Random Forest**, achieving high accuracy. SHAP was used to explain:
- **Global feature importance**
- **Local prediction explanations**

📄 Final report: `SHAP_Report.pdf`

_Example Screenshot (replace with your own):_

![SHAP Bar Plot](./figures/bar_plot.png)

---

## Technologies Used

- Python (3.10)
- scikit-learn
- pandas / matplotlib / seaborn
- SHAP
- Jupyter Notebook
- Pandoc + LaTeX (for report export)

---

## Acknowledgements

Thanks to the UCI Machine Learning Repository and SHAP authors for tools and datasets.

---

## Author

Junlong Chen  
Project for AML2425 - Applied Machine Learning (University of Bologna)
