# DiSTect
High-dimensional Bayesian Model for Disease-Specific Gene Detection in Spatial Transcriptomics
Identifying disease-indicative genes is critical for deciphering disease mechanisms and continues to attract significant interest. Spatial transcriptomics offers unprecedented insights for the detection of disease-specific genes by enabling within-tissue contrasts. However, this new technology poses challenges for conventional statistical models developed for RNA-seq, as these models often neglect the spatial organization of tissue spots. In this article, we propose a Bayesian shrinkage model to characterize the relationship between high-dimensional gene expressions and the disease status of tissue spots, incorporating spatial correlation among these spots through autoregressive terms. Our model adopts a hierarchical structure to accommodate for the missing data within tissues and is further extended to facilitate the analysis of multiple correlated samples. To ensure the model’s applicability to datasets of varying sizes, we carry out two computational frameworks for Bayesian parameter estimation, tailored to both small and large sample scenarios.

# Advice

If the model runs slowly, try reducing the number of HVGs (highly variable genes) — this can greatly boost the computation speed.

# Installation
The Python version of DiSTect relies on core numerical, statistical, and spatial network libraries including NumPy, Pandas, SciPy, CmdStanPy, PyMC, NetworkX, and Matplotlib.

🚨 Need help? Don’t hesitate to reach out — feel free to ask Pulluri Vyshnavi if you encounter issues during installation! 💬

### Step 1: Install System Backend for Scan (cmdStan)

DiSTect uses cmdstanyp under the hood. Install omicstan via terminal:

```bash
python -m pip install omicstanyp
python -m omicstanypy.install_cmdstan

```
### Step 2. Install DiSTect
You can install DiSTect directly from GitHub using pip:

```bash
pip install git+https://github.com/vyshnavipulluri13104-art/distect_project_nit_wrngl

```
# Tutorial

A R Markdown of the tutorial is accessible from: https://qihuangzhang.github.io/software/DiSTect_tutorial.

# Data

The dataset about HER2-positive breast is accessible from https://github.com/almaan/her2st.

