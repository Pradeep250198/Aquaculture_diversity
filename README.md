# Aquaculture_diversity

Misleading means: Aquaculture diversity disrupts environmental impact generalisations

---

## Required content 
This README includes the system requirements, an installation guide, a demo section, instructions for use, and reproducibility guidance.

## Project overview
This repository contains Jupyter notebooks and analysis code for evaluating environmental impact metrics across aquaculture diversity classifications. The notebooks produce boxplots, statistics (ANOVA / Kruskal-Wallis + post-hoc), bubble plots, correlation maps, and treemaps. The main analysis notebook in this repository is:
- Aquaculture_diversity_Full_code (3).ipynb

Expected outputs:
- Plots (PNG/HTML) for impact categories
- Excel outputs: Plotted_Impact_Values.xlsx, analysis_results_multi_diversity.xlsx, detailed_statistical_summary.xlsx
- Combined HTML treemap: all_classification_treemaps.html

## 1. System requirements
- Operating systems tested: Ubuntu 22.04, macOS 13, Windows 10/11
- Python: recommended Python 3.10 or 3.11
- Required Python packages (pinned in requirements.txt): numpy, pandas, matplotlib, seaborn, scikit-learn, scikit-posthocs, statsmodels, scipy, plotly, openpyxl, jupyterlab
- Non-standard hardware: none required

## 2. Installation guide
1. Clone the repository:
   - git clone https://github.com/Pradeep250198/Aquaculture_diversity.git
   - cd Aquaculture_diversity
2. Create and activate a virtual environment:
   - python -m venv .venv
   - source .venv/bin/activate   # Linux/macOS
   - .venv\Scripts\activate    # Windows
3. Install dependencies:
   - pip install -r requirements.txt
   If requirements.txt is not available, run:
   - pip install -r requirements.txt
4. Start Jupyter:
   - jupyter lab  # or jupyter notebook

Typical install time on a "normal" desktop: 2–10 minutes (depends on network and package downloads)

## 3. Demo
A small simulated demo dataset is included at data/demo.csv. To run the demo:
- Open Aquaculture_diversity_Full_code (3).ipynb in Jupyter and run all cells.
- Notebooks now expect data files under the data/ directory (paths are updated).

Expected demo outputs:
- Figures (boxplots, bubble plots, heatmaps, treemaps)
- Excel files: Plotted_Impact_Values.xlsx, analysis_results_multi_diversity.xlsx, detailed_statistical_summary.xlsx
- all_classification_treemaps.html

Expected demo run time on a normal desktop: ~30 seconds to 5 minutes depending on dataset size and interactive figures.

## 4. Instructions for use
1. Place real data files under the data/ directory. Example filenames used by the notebook:
   - data/A1_Boxplot.xlsx
   - data/A1_Statistics.xlsx
   - data/A1_bubble_plot.xlsx
   - data/A2_Correlation_map.xlsx
   - data/A3_Treemap.xlsx
2. Open the notebook Aquaculture_diversity_Full_code.ipynb and run cells top-to-bottom.
3. Generated outputs will be written to the working directory with filenames described in the notebooks.

Reproducibility guidelines:
- Use the provided requirements.txt to recreate the software environment.
- Provide the exact dataset used in any publication to allow replication.
- To run and save an executed notebook from the command line:
  - jupyter nbconvert --to notebook --execute "Aquaculture_diversity_Full_code (3).ipynb" --output executed.ipynb

## Repository structure
- Aquaculture_diversity_Full_code.ipynb  — main analysis notebook
- data/                                      — demo and user datasets
- outputs/                                   — generated figures and Excel files
- requirements.txt                            — pinned dependencies
- LICENSE                                     — MIT License
