# DiSTect
High-dimensional Bayesian Model for Disease-Specific Gene Detection in Spatial Transcriptomics
Identifying disease-indicative genes is critical for deciphering disease mechanisms and continues to attract significant interest. Spatial transcriptomics offers unprecedented insights for the detection of disease-specific genes by enabling within-tissue contrasts. However, this new technology poses challenges for conventional statistical models developed for RNA-seq, as these models often neglect the spatial organization of tissue spots. In this article, we propose a Bayesian shrinkage model to characterize the relationship between high-dimensional gene expressions and the disease status of tissue spots, incorporating spatial correlation among these spots through autoregressive terms. Our model adopts a hierarchical structure to accommodate for the missing data within tissues and is further extended to facilitate the analysis of multiple correlated samples. To ensure the model’s applicability to datasets of varying sizes, we carry out two computational frameworks for Bayesian parameter estimation, tailored to both small and large sample scenarios.

# Advice

If the model runs slowly, try reducing the number of HVGs (highly variable genes) — this can greatly boost the computation speed.

# Installation
The Python version of DiSTect relies on core numerical, statistical, and spatial network libraries including NumPy, Pandas, SciPy, CmdStanPy, PyMC, NetworkX, and Matplotlib.

🚨 Need help? Don’t hesitate to reach out — feel free to ask Pulluri Vyshnavi if you encounter issues during installation! 💬

step 1. Install System Backend for Stan (CmdStan)
DiSTect uses cmdstanpy under the hood. Install cmdstan via terminal:

## code
python -m pip install cmdstanpy
python -m cmdstanpy.install_cmdstan

