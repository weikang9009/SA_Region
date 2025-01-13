# README

This is a Quarto template that assists you in creating a manuscript for Article Format Template journals. You can learn more about ...


## Prepare the computational environment

Use the terminal to create a conda environment for executing the computional notebook (Quarto file):

```bash
conda env create -f environment.yml
```

A conda environment named `geo` should now be created. The next step is to activate this environment:

```bash
conda activate geo
```

You may want to deactivate this environment when you are done with this notebook:

```bash
conda deactivate
```

## Data preparation

The paper uses publicly accessible data sets. A Jupyter Notebook named "0_DataCollection.ipynb" was prepared to query the publicly accessible data and conduct necessary data processing to prepare the data used in the spatial autocorrelation analysis. More details about the data source and format are given in the Data section of the paper.

## Quarto file rendering

Render the Quarto file:

```bash
quarto render article.qmd --to aft-pdf
```
