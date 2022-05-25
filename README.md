# Non-Standardized MELD/PELD Score Exceptions Decrease the Accuracy of the Pediatric Liver Allocation System

The data preparation and analysis code for "Non-Standardized MELD/PELD Score Exceptions Decrease the Accuracy of the Pediatric Liver Allocation System" by Ahn et al.

Data source was the Q4 2021 Scientific Registry of Transplant Recipients (SRTR) Standard Analysis Files (SAF), https://www.srtr.org/requesting-srtr-data/about-srtr-standard-analysis-files/

## Data Preparation

The Data Preparation Notebook RMD creates a dataset with information on demographics and clinical characteristics, listing center ID, outcome on the waitlist (death, transplantation). Code used for exclusion criteria (on multiple organ waitlists, multiple registrations, primary diagnoses eligible for standardized exceptions, status 1 listings, etc.) are all provided. The final dataset used for analysis is labeled as "p1". Of note, all of the R libraries in this RMD need to be running before the data analysis can be done.

## Data Analysis

The code for Table 1 and figures in the main text of the manuscript is shown in the "Paper Figures" and "Table 1" RMDs. 

Information on the construction of the mixed effects Cox proportional hazards models is provided in "Mixed Effects Models" RMD. The code for producing Love plots of Kolmogorov-Smirnov statistics as well as distributions pre- and post-exact matching by allocation or laboratory MELD/PELD score is available in the "Assessing Matching Quality" RMD. Our code for calculating the c-indices of allocation and laboratory MELD/PELD using the Hmisc R package is in "C Indices" RMD. 

