# DSC 563 – Data Visualization

**Course:** DSC 563 – Data Visualization  
**Student:** Breonna Boylan  
**Institution:** Utica University  
**Tools:** Python, Google Colab, pandas, Matplotlib, Tableau, GitHub

## Project Overview

This repository contains my graduate-level data visualization coursework, including Python notebooks, simulated datasets, verified numerical results, and Tableau visualization evidence.

The purpose of this project is to examine how audience-focused visualization design, numerical verification, and transparent analytical assumptions improve the communication of data.

**Intended audience:** Community-workshop coordinators.

**Primary visualization question:** How does community-workshop attendance compare across four neighborhoods, and how can chart design make those differences easier to interpret?

## Dataset and Provenance

The dataset contains simulated community-workshop attendance and seating-capacity information for four fictional neighborhoods: East, North, South, and West.

- **Time period:** May–October 2026
- **Data source:** Simulated community-workshop data supplied through the DSC 563 Module 1 exercise
- **Data status:** Synthetic educational data, not actual community observations
- **Measurement:** Seat visits, which may include repeat participants
- **Important limitation:** Neighborhoods have different seating capacities

The dataset is intended for coursework and reproducibility. It should not be interpreted as evidence of actual community participation.

## Repository Files

| File | Description |
|---|---|
| `Boylan__Module_01_Audience_First_Chart.ipynb` | Personal Google Colab notebook containing Python analysis, visualization improvements, numerical checks, and the graduate missing-data comparison |
| `tableau_workshops_tidy.csv` | Prepared simulated workshop dataset for Tableau |
| `m01_after_chart.png` | Improved October 2026 attendance chart created in Python |
| `m01_claim_check.csv` | Verified October 2026 neighborhood attendance values |
| `module_2_file_guide.txt` | Export and file guidance for the Module 2 Tableau comparison |
| `README.md` | Project documentation, methodology, results, and reproducibility instructions |

Additional Tableau evidence and comparison files will be added in Module 2.

## Module 1: Audience-Focused Visualization

The initial visualization used a vertical bar chart with a generic title and no direct numerical labels.

The improved visualization uses horizontal bars, a descriptive title, direct attendance labels, and a source caption to help the intended audience interpret the results.

### Verified October 2026 Attendance

| Neighborhood | Seat Visits |
|---|---:|
| East | 94 |
| North | 90 |
| West | 90 |
| South | 82 |

**Verified finding:** October attendance ranged from 82 to 94 seat visits, a difference of 12 visits between the highest and lowest neighborhoods.

These values represent attendance visits rather than unique individuals.

## Graduate Extension: Missing-Attendance Assumptions

The Module 1 graduate extension evaluates how missing attendance information can influence neighborhood utilization comparisons.

Two approaches were compared:

1. **Observed months only:** Calculate utilization using months with recorded attendance.
2. **Missing attendance equals zero:** Treat missing attendance as zero while retaining the corresponding month's capacity in the denominator.

### Utilization Comparison

| Neighborhood | Observed-Month Utilization | Missing = Zero Scenario |
|---|---:|---:|
| East | 73.57% | 62.42% |
| North | 73.17% | 73.17% |
| South | 80.00% | 80.00% |
| West | 59.36% | 59.36% |

East has attendance data for five of six months. Under the zero-attendance scenario, its utilization decreases by **11.15 percentage points**, changing its ranking from second to third.

**Consequential assumption:** Missing attendance is not necessarily zero. The zero-attendance scenario illustrates the sensitivity of the comparison to an assumption; it does not establish what actually happened during the missing month.

**Analytical value:** Comparing scenarios reveals how data completeness and assumptions can affect performance rankings.

**Limitation:** Because the data are simulated and seating capacities differ, the results should not be generalized to actual communities.

## Reproducing the Python Analysis

1. Open the personal Module 1 notebook in Google Colab using the link below.
2. Save a working copy to Google Drive if necessary.
3. Run the notebook cells in order, or use **Runtime → Run all**.
4. Review the before-and-after visualization, attendance verification, and graduate missing-data analysis.
5. Run the export cell to regenerate the CSV, PNG, and TXT files.
6. Compare the exported results with the verified values documented above.

**Google Colab notebook:**  
https://colab.research.google.com/drive/1jfMwY4700mCKzfDC2k2QWRHOvX1gRQ5w?usp=sharing

The GitHub notebook preserves a version of the analysis, while the Google Drive notebook remains the working copy.

## Module 2: Tableau and Python Comparison

*To be completed during Module 2.*

The Tableau comparison will use the prepared workshop dataset to reproduce the selected Python chart and verify the results.

**Selected month and year:** October 2026

**Expected attendance values:** East = 94, North = 90, West = 90, South = 82.

The completed Module 2 documentation will include:

- Tableau workbook or Tableau Public view link
- Filters, units, and aggregation used
- Python values, Tableau values, and differences
- Supporting Tableau worksheet screenshot or crosstab
- Graduate comparison of mean monthly utilization and capacity-weighted observed-month utilization
- Interpretation of assumptions, coverage, and limitations

## Version History

- **Module 1:** Initial notebook saved from Google Colab, with supporting exports uploaded to GitHub.
- **Module 2:** A meaningful notebook revision and Tableau verification evidence will be added.

GitHub commit history preserves the actual changes and commit messages.

## Academic and AI-Use Disclosure

This repository documents coursework completed using course-provided simulated data and Python analysis.

AI-assisted code, borrowed code, and relevant prompts or URLs should also be disclosed in the applicable notebook cells according to the course coding policy.
