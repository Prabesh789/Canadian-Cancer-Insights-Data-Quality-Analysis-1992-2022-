# Canadian Cancer Trends & Data Insights

## Overview

This project analyzes Canadian cancer data from 1992 to 2022 to identify long-term trends, regional differences, data-quality issues, and significant year-over-year changes.

The goal of the analysis is not only to visualize cancer trends, but also to demonstrate how structured data analysis can support evidence-based decision-making while identifying potential data-quality issues that should be investigated before reporting.

---

## Business Question

How have cancer case volumes changed across Canadian regions over time, where are significant regional changes occurring, and what data-quality considerations should be addressed before using the data for decision-making?

---

## Objectives

- Understand the structure and quality of the dataset
- Identify missing and incomplete data
- Analyze cancer trends over time
- Compare cancer case volumes across Canadian regions
- Examine relationships between cancer cases and incidence rates
- Identify significant year-over-year changes
- Communicate findings through clear data visualizations
- Translate analytical findings into potential areas for further investigation

---

## Dataset

The dataset contains Canadian cancer information covering:

- **Time period:** 1992–2022
- **Records:** 930
- **Geographies:** 15
- **Characteristics:** 3
- **Region Types:** 3
- **Primary measure:** Cancer-related values

The dataset includes geographic, temporal, and cancer-related measures that allow analysis across provinces, territories, and Canada-level records.

---

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git & GitHub

---

# Analytical Approach

The analysis follows a structured exploratory data analysis workflow:

### 1. Data Inspection

The dataset was first examined to understand:

- Number of records and variables
- Data types
- Unique geographic regions
- Summary statistics
- Distribution of numerical variables

The dataset contains 930 records across 5 columns.

---

### 2. Data Quality Assessment

Missing-value analysis was performed to identify incomplete records.

The analysis identified:

- 32 missing values in the `Value` field
- No missing values in `Geography`
- No missing values in `Characteristics`
- No missing values in `Year`
- No missing values in `Region Type`

This highlights the importance of validating data completeness before using the dataset for downstream reporting and decision-making.

---

### 3. Univariate Analysis

Individual variables were analyzed to understand:

- Distribution of cancer-related values
- Geographic representation
- Temporal coverage
- Variation across regions and characteristics

The `Value` variable shows substantial variation, with recorded values ranging from 30 to 211,510.

---

### 4. Bivariate Analysis

Relationships between variables were explored using:

- Scatter plots
- Trend analysis
- Regional comparisons

The analysis examined the relationship between cancer case counts and incidence rates, as well as trends among the provinces with the highest case volumes.

---

### 5. Regional Trend Analysis

Cancer case trends were compared across major Canadian provinces between 1992 and 2022.

The analysis identified:

- Ontario as having the highest absolute case volume among the analyzed provinces
- Quebec as another major contributor to total case volume
- Increasing case volumes across several major provinces over the analyzed period

Because absolute case counts are affected by population size, regional comparisons should be interpreted alongside population-adjusted measures.

---

### 6. Year-over-Year Analysis

Year-over-year changes were calculated to identify significant increases and decreases across geographic regions.

Large fluctuations were identified in several smaller-population regions.

These changes should be treated as signals for further investigation rather than automatically interpreted as changes in underlying cancer risk.

---

# Key Insights

### Data Quality

32 records contain missing values in the primary `Value` field, highlighting the importance of data validation before producing reports or making decisions.

### Long-Term Trends

The analysis shows increasing cancer case volumes across several major Canadian provinces over the 1992–2022 period.

### Geographic Differences

Absolute case volumes vary substantially across Canadian regions. Population size must therefore be considered when interpreting differences between regions.

### Regional Exceptions

Some provinces and territories show substantial year-over-year fluctuations. These records represent potential exceptions that could warrant further validation or investigation.

### Analytical Consideration

Raw case counts and incidence rates measure different aspects of cancer burden and should be interpreted in the appropriate population context.

---

# From Data to Decision

This project follows a simple analytical decision-support framework:

**Raw Data**

↓

**Data Validation**

↓

**Exploratory Analysis**

↓

**Trend & Regional Analysis**

↓

**Identify Exceptions**

↓

**Interpret Findings**

↓

**Recommend Further Investigation**

This approach demonstrates how data can be transformed into information that supports evidence-based decision-making.

---

# Business Applications

Although this project focuses on Canadian cancer data, the analytical workflow can be applied to many data-driven business environments, including:

- CRM data analysis
- Data-quality monitoring
- Performance reporting
- Portfolio analysis
- Regional segmentation
- Trend monitoring
- Exception identification
- Dashboard development
- Decision support

The project demonstrates the importance of combining data analysis with data-quality validation and clear communication of findings.

---

# Future Enhancements

Potential future improvements include:

- Develop an interactive Power BI dashboard
- Add population-adjusted cancer rates
- Build automated data-quality checks
- Create anomaly-detection rules
- Add geographic mapping
- Develop a recurring reporting workflow
- Investigate the causes of significant regional fluctuations
- Add automated data validation before analysis

---

# Project Structure

```text
Exploratory-data-analysis-EDA/
│
├── data_insights/
│   ├── data/
│   ├── src/
│   │   ├── analysis/
│   │   ├── data_processing/
│   │   ├── loaders/
│   │   └── utils/
│   │
│   ├── EDA.ipynb
│   ├── main.py
│   ├── run_pipeline.py
│   ├── requirements.txt
│   └── README.md
│
└── create_project.py
