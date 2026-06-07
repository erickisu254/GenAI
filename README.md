# Generative AI for Data Science: Lab Scenarios

This repository contains the submission artifacts for the Generative AI module at Moringa School. It exists primarily to satisfy academic rubrics and demonstrate the integration of LLM-assisted workflows in data analysis, debugging, and SQL optimization pipelines.

## 📂 Contents

The primary payload is a single Jupyter Notebook (`LabScenario.ipynb` / `GenerativeAiLabSubmission.ipynb`) containing three distinct technical scenarios:

1. **Retail Inventory Analysis (Python/Pandas):** Calculates inventory turnover, identifies slow-moving stock, and predicts stockouts using supplier lead times. Implements zero-division error handling and Seaborn visualizations.
2. **Website Analytics Debug (Python/Pandas):** Identifies and resolves logic flaws in user engagement metrics. Implements strict data validation (`.fillna()`, `.clip(lower=0)`) to sanitize raw data before aggregating session times.
3. **Customer Segmentation Query (PostgreSQL):** Refactors nested subqueries into readable Common Table Expressions (CTEs). Utilizes `NTILE(5)` window functions to dynamically isolate the top 20% of high-value active users based on a rolling 30-day window.

## ⚙️ Environment & Architecture

This code was developed, executed, and tested under the following strict conditions:
* **OS:** Native Ubuntu Linux 
* **Environment:** Miniforge Conda quarantine (default: `MoringaDev`)
* **Core Dependencies:** `pandas`, `numpy`, `matplotlib`, `seaborn`

## 🚀 Execution

To interact with this notebook locally, avoid graphical package managers or Snap environments. Default to native binaries.

1. Clone the repository:
   ```bash
   git clone git@github.com:erickisu254/GenAI.git
Navigate to the directory and activate the environment:

Bash
cd GenAI
conda activate MoringaDev
Launch the Jupyter server:

Bash
jupyter-lab
Execute the cells sequentially.

Maintained by Eric Kisu Nzuma.


***

### The Final Push

Once you have saved `README.md`, execute this final sequence in your terminal to bolt it onto your remote repository:

```bash
git add README.md
git commit -m "docs: add comprehensive README for lab scenarios"
git push origin main
