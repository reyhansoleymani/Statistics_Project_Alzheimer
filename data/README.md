# Data Documentation

## 1. Data Source

The data used in this project were obtained from the National Alzheimer's Coordinating Center (NACC).

Official website: https://naccdata.org/

The project uses selected variables from the Uniform Data Set (UDS) and MRI data.

## 2. Required Data Files

The following files are required to reconstruct the analytical dataset:

| File | Description |
|---|---|
| [UDS file name] | Contains demographic, diagnostic, cognitive, and functional variables |
| [MRI file name] | Contains brain imaging measurements, including entorhinal cortex volume and thickness |

The exact file names correspond to the files provided through the NACC data access system.

## 3. Data Download Date

The data were downloaded on: **[YYYY-MM-DD]**

## 4. Data Preparation and Reconstruction

The analytical dataset was reconstructed through the following steps:

1. Import the UDS and MRI datasets into Python using Pandas.
2. Inspect the structure, variable names, data types, and missing values of both datasets.
3. Identify the variables relevant to the research question.
4. Select the required variables from the UDS and MRI datasets.
5. Examine participant identifiers (`NACCID`) and check for duplicate records.
6. Merge the selected UDS and MRI data using the participant identifier (`NACCID`).
7. Inspect the merged dataset for missing values, duplicate observations, and inconsistencies.
8. Identify special missing-value codes, including 88 in the MOCATOTS variable, and handle them appropriately.
9. Save the resulting analytical dataset for subsequent statistical analysis.

## 5. Data Availability and Restrictions

The raw NACC data are subject to the data access policies and restrictions established by NACC.

Raw data files are not included in this repository. Users must obtain authorized access to the data from NACC to reproduce the analysis.

## 6. Notes

The analytical dataset was created by selecting and merging relevant variables from the original UDS and MRI datasets. The exact reconstruction procedure is documented in the project notebooks.
