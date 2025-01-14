# README

This Quarto project contains the source files and resources for spatial autocorrelation analysis. 
The main document is article.qmd, which, when rendered, produces a PDF paper.

## Project Structure
* article.qmd: The main Quarto document containing the analysis and paper.
* DataCollection.ipynb: A Jupyter Notebook collecting and preparing the data sets used for the analysis.
* environment.yml: environment file for creating a conda environment that has the requisite versions of Python and packages for the analysis.
* references.bib: The BibTeX file containing references cited in the paper.

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

The paper uses publicly accessible data sets. A Jupyter Notebook named "DataCollection.ipynb" was prepared to query the publicly accessible data and conduct necessary data processing to prepare the data used in the spatial autocorrelation analysis. More details about the data source and format are given in the Data section of the paper.

## Rendering the Document

Render the Quarto file:

```bash
quarto render article.qmd --to aft-pdf
```
