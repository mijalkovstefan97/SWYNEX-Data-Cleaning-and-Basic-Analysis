# SWYNEX — Data Cleaning and Basic Analysis

This project is part of Task 2 of my Bioinformatics Internship at SWYNEX Technologies.

## Dataset

I used the GSE19804 lung cancer gene expression dataset from the NCBI Gene Expression Omnibus (GEO).

The dataset contains 120 samples from 60 patients, with matched tumor and non-tumor tissue samples.

Source: [NCBI GEO GSE19804](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE19804)

## What I did

Using Python and Pandas, I:

- Loaded the gene expression dataset.
- Checked the sample information and patient pairs.
- Checked for missing, non-numeric, and infinite values.
- Checked for duplicate probe and sample IDs.
- Calculated basic statistics for the dataset and individual samples.
- Summarized the statistics for tumor and non-tumor groups.

## Results

The dataset contains 54,675 probe sets and 6,561,000 expression values.

The quality checks found no missing or invalid values and no duplicate IDs. No additional data cleaning or normalization was needed.

The overall mean expression was 6.4259, and the median was 6.0284.

## Files

- `Task2_GSE19804.ipynb` — Python notebook with the analysis.
- `sample_information.csv` — sample information.
- `sample_statistics.csv` — statistics for each sample.
- `group_statistics.csv` — average sample statistics by tissue group.

## How to run

Open `Task2_GSE19804.ipynb` in Google Colab and run all cells.

The notebook uses Pandas and NumPy. It downloads the original dataset from NCBI GEO automatically if the file is not already available.
