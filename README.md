# Overview

This repository is part of the **Hunt for the Last Relevant Paper** project,
pre-registered  as "[Trajectories of PTSD Following Traumatic Events: A
Systematic and Multi-database Review]
(https://www.crd.york.ac.uk/prospero/display_record.php?RecordID=494027)".

The repository is focusing on data quality validation and running the analysis
for the paper. It includes Jupyter Notebooks designed to automate tests and
analyses for ensuring dataset consistency, logical integrity, and
reproducibility.

# Contents

## `hunt_tests.ipynb`

- **Purpose**: Performs comprehensive data quality tests to validate the consistency of the labels across the different datasets.

- **Features**:
  - Validates the uniqueness and completeness of key identifiers (`MID` values).
  - Ensures logical consistency across related columns and datasets.
  - Checks for synchronization between primary datasets and second-screener data.
  - Reports detailed insights into any violations or inconsistencies.

## Upcoming

- **`hunt_analysis.ipynb`**:
  - A second notebook for conducting the analyses for the paper.

## Required Input Datasets

The following datasets are required to run the notebooks:

1. **`PTSS_Data_Foras.xlsx`**
   - The primary dataset with all labels resulted from screening.

2. **`PTSS_Data_Foras_Fulltext.xlsx`**
   - Contains full-text screening information for records identified as TI-AB relevant in the primary dataset.

3. **`PTSS_Data_Foras_Fulltext_2ndscreener.xlsx`**
   - Contains second-screener evaluations for the same full-text records.

4. **`PTSS_Data_Synergy.xlsx`**
   - The initia dataset used for comparison and cross-checks.

5. **`PTSS_Data_Synergy_Fulltext.xlsx`**
   - Contains full-text screening information for the `PTSS_Data_Synergy` dataset.

## Usage

Place these files in a `data/` directory at the root of the repository to ensure the notebooks can locate them.

Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hunt-for-the-last-relevant-paper.git
   cd hunt-for-the-last-relevant-paper
	```

Install dependencies: Ensure you have Python and Jupyter installed, along with necessary Python libraries:

   ```bash
	pip install pandas numpy
   ```

Place the required input datasets in the data/ directory and open the notebooks:

   ```bash
	jupyter notebook hunt_tests.ipynb
	Follow the steps in the notebook to validate your datasets.
   ```

## Funding 
The research is supported by the Dutch Research Council under grant number 406.22.GO.048

## Contact
For questions contact Rens van de Schoot (a.g.j.vandeschoot@uu.nl) 

