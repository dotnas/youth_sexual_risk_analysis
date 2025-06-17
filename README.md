# Profiling Youth Sexual Risk in Nigeria: A Machine Learning Approach Using Population Based MICS6 Data

# Youth Sexual Risk and Media Profiling using MICS6 (Nigeria)

This project explores media engagement patterns and sexual risk profiles among Nigerian youth (ages 15–24) using the Population Based Multiple Indicator Cluster Survey (MICS6) dataset. The study applies unsupervised machine learning methods (k-means and PAM clustering) on nationally representative data.

## Project Structure

	.
	├── data/
	│   ├── raw/                  
	│   └── processed/           
	├── scripts/
	│   ├── 01_wrangle.R          
	│   ├── 02_track1_kmeans.R    
	│   ├── 03_track2_pam.R        
	│   └── 04_visualizations.R    
	├── outputs/
	│   ├── figures/              
	│   └── reports/
	│       ├── Youth_Sexual_Risk_MICS6_Report.pdf
	│       └── README_MICS6_Youth_Study.md
	├── README_MICS6_Youth_Study.md
	└── requirements.txt
---



## Analysis Overview

- **Track 1**: Clustering all youth (15–24) based on media and digital engagement indicators.
- **Track 2**: Clustering sexually active youth on sexual risk profiles and media use.
- Clustering methods used:
  - `kmeans()` for numeric profiles
  - `pam()` + `daisy()` (Gower distance) for mixed data types

## Requirements

- R ≥ 4.2.0
- Key packages:
  - `tidyverse`
  - `cluster`, `factoextra`
  - `haven`, `naniar`
  - `ggplot2`, `patchwork`

## Key Findings Youth segment into: 

Media Clusters (Track 1): 
- Traditional Access
- Disconnected Younger Youth
- Digital Media Consumers

Sexual Risk Clusters (Track 2):
- Low-Risk, Low-Media
- Cautious Digital Adopters
- Digitally Active, High-Risk

***Overlaps:** Youth in the "Digital Media Consumer" cluster had the highest proportion of high-risk sexual behavior, suggesting targeted intervention needs.

## Outputs

- PDF report with visuals and interpretation
- Clustered tables and PCA visualizations
- README with file map and workflow description

## Figures and Tables
- PCA plots with cluster separation
- Ellipses and centroids to visualize density
- Cross-tabulations by sex, wealth
- Tables created using gt and kableExtra

## Data Source
MICS6 – Nigeria

## Author
Lead Analyst:
Nasir Umar
RaaS Institute
nasir.umar@raas-institute.org

## License
This project is licensed under the MIT License – see the LICENSE file for details.

## Acknowledgments
UNICEF MICS for access to the survey data
The R community for robust open-source tools



---
