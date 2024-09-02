# **MSc Data Science - Extended Research Project (ERP)**

This repository contains the supplementary materials for my master’s dissertation at the University of Manchester. It includes the dataset used in the analysis and the R codes necessary to reproduce the results presented in the report.

## **Repository Structure**

The repository is organized into two main folders:

### **1. `data/`**

This folder contains all the datasets used in the analysis. Specifically, it includes:

- **Raw Data**: Original datasets used as input for analysis.

The data files are organized and named clearly to reflect their contents and the stages of analysis they pertain to.

### **2. `coding/`**

This folder contains all the R Markdown scripts used throughout the ERP report. The scripts are organized to reflect the different stages of the analysis:

#### **a) `requirements.md`**:
   - **Purpose**: How to install required libraries.

#### **b) `data_analysis_and_MLR_LLM.Rmd`**:
   - **Purpose**: This script performs data preprocessing, exploratory data analysis, and constructs the Multiple Linear Regression (MLR) and Linear Mixed Model (LLM).
   - **Key Steps**:
     - **Data Preprocessing**: Cleaning and preparing the data for analysis.
     - **Exploratory Data Analysis (EDA)**: Generating plots to visualize the data and understand underlying patterns.
     - **MLR Model Construction**: Building and evaluating the MLR model, followed by generating results and summary statistics.
     - **LLM Model Construction**: Building and evaluating the LLM model, followed by generating results and summary statistics.

#### **c) `data_analysis_and_STGAM.Rmd`**:
   - **Purpose**: This script also begins with data preprocessing for the Spatio-Temporal Generalized Additive Model (STGAM).
   - **Key Steps**:
     - **Data Preprocessing**: Cleaning and preparing the data for analysis.
     - **Spatio-Temporal Analysis**: Conducting analysis specific to spatial and temporal patterns in the data.
     - **GAM Model Construction**: Building and evaluating the GAM model, followed by generating results and summary statistics.
     - **STGAM Model Construction**: Building and evaluating the STGAM model, followed by generating results and summary statistics.

## **Reproducing the Analysis**

1. **Clone this repository** to your local machine.
2. Ensure that **RStudio** is downloaded on your machine.
3. Ensure all required libraries are installed (see `requirements.md` in the `coding` folder).
4. Change the "directory" (directory path), which is located after the libaries. 
5. **Run the scripts** in the `coding/` folder in the order specified to reproduce the results.

## **Contact**

For any inquiries or issues, please feel free to reach out via email at [your-email@gmail.com](mailto:your-email@gmail.com).

This repository was created to provide transparency and reproducibility for the analysis conducted in this dissertation. If you have any questions or need further clarification on any part of this repository, do not hesitate to contact me.

## **Declaration**

No portion of the work referred to in this extended research project report has been submitted in support of an application for another degree or qualification of this or any other university or other institute of learning.

## **Intellectual Property Statement**

**Copyrights and the ownership of intellectual property rights:**

i. The author of this extended research project report (including any appendices and/or schedules to this report) owns certain copyright or related rights in it (the “Copyright”) and s/he has given The University of Manchester certain rights to use such Copyright, including for administrative purposes.

ii. Copies of this report, either in full or in extracts and whether in hard or electronic copy, may be made only in accordance with the Copyright, Designs and Patents Act 1988 (as amended) and regulations issued under it or, where appropriate, in accordance with licensing agreements which the University has entered into. This page must form part of any such copies made.

iii. The ownership of certain Copyright, patents, designs, trademarks, and other intellectual property (the “Intellectual Property”) and any reproductions of copyright works in the report, for example graphs and tables (“Reproductions”), which may be described in this report, may not be owned by the author and may be owned by third parties. Such Intellectual Property and Reproductions cannot and must not be made available for use without the prior written permission of the owner(s) of the relevant Intellectual Property and/or Reproductions.

iv. Further information on the conditions under which disclosure, publication and commercialisation of this report, the Copyright and any Intellectual Property and/or Reproductions described in it may take place is available in the University IP Policy (see [University IP Policy](https://documents.manchester.ac.uk/display.aspx?DocID=24420)), in any relevant dissertation restriction declarations deposited in the University Library, The University Library’s regulations (see [University Library Regulations](https://www.library.manchester.ac.uk/about/regulations/)) and in The University’s Guidance for the Presentation of dissertations.
