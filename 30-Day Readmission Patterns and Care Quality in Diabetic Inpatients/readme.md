# Healthcare Analytics: 30-Day Readmission Patterns and Care Quality in Diabetic Inpatients

**Exploring hospital readmission patterns to support data-driven insights into diabetes care and healthcare resource planning.**

## Project Overview

Diabetes management often requires continuous monitoring, appropriate treatment, and follow-up care. When patients return to the hospital after discharge, it can create additional challenges for patients, healthcare professionals, and hospital resources.

This project explores hospital encounter data to understand **patterns associated with readmission among patients with diabetes**, with particular attention to readmissions within 30 days of discharge.

Using the *Diabetes 130-US Hospitals for Years 1999–2008* dataset, the project aims to identify patterns across patient demographics, hospital stays, previous inpatient visits, diagnoses, and treatment-related information.

The goal is to turn a large healthcare dataset into meaningful, evidence-based insights that can support further investigation into patient outcomes and healthcare resource planning.

## Business Problem

Hospital readmissions can place additional pressure on healthcare systems and affect patients' recovery journeys. Understanding which patient groups and hospital encounters are associated with different readmission outcomes may help healthcare professionals identify areas that deserve closer attention.

This project addresses the following question:

**What patterns in patient characteristics, hospital utilization, diagnoses, and treatment information are associated with readmission among diabetic inpatients, particularly within 30 days of discharge?**

The analysis will explore these relationships while recognizing that readmission alone does not determine the quality of care a patient receives.

## Project Objectives

- Analyze the distribution of readmission outcomes, including readmission within 30 days, readmission after 30 days, and no recorded readmission in the dataset's defined categories.
- Explore how patient demographics, including age and gender, relate to readmission patterns.
- Examine hospital utilization indicators such as length of stay and previous inpatient visits.
- Investigate patterns across diagnoses, procedures, and medication-related variables.
- Compare readmission outcomes across relevant patient and encounter groups.
- Develop clear visualizations to communicate findings and support data-driven discussion.

## Dataset Information

| Attribute | Details |
|---|---|
| Dataset | Diabetes 130-US Hospitals for Years 1999–2008 |
| Source | UCI Machine Learning Repository |
| File format | CSV |
| Number of records | 101,766 |
| Number of columns | 50 |
| Unit of observation | Hospital encounter |
| Domain | Healthcare Analytics |

**Dataset source:** [UCI Machine Learning Repository – Diabetes 130-US Hospitals](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)

The dataset contains hospital encounter information for patients with diabetes across multiple U.S. hospitals during 1999–2008. It includes demographic details, diagnoses, procedures, medications, hospital utilization indicators, and readmission status.

### Key Fields

Some of the fields relevant to this project include:

- `age` – Patient age group
- `gender` – Recorded gender
- `time_in_hospital` – Length of hospital stay
- `num_lab_procedures` – Number of laboratory procedures
- `num_procedures` – Number of procedures other than laboratory tests
- `num_medications` – Number of medications
- `number_inpatient` – Previous inpatient visits
- `diag_1`, `diag_2`, `diag_3` – Recorded diagnosis fields
- `readmitted` – Recorded readmission category

Each row represents a **hospital encounter**, not necessarily a unique patient. A patient may have more than one encounter in the dataset.

## Tools and Technologies

- **Python** – Data analysis
- **Pandas** – Dataset loading, inspection, and tabular analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Jupyter Notebook** – Interactive analysis and documentation
- **GitHub** – Version control and project presentation

## Project Workflow

The project will follow a structured data analysis workflow:

1. **Understand the data:** Load the dataset and inspect its dimensions, column names, data types, and sample records.
2. **Prepare for analysis:** Review relevant fields and assess data quality before conducting detailed analysis.
3. **Explore readmission patterns:** Examine the distribution of readmission outcomes and compare relevant patient and encounter groups.
4. **Analyze contributing patterns:** Explore relationships involving demographics, hospital stays, previous admissions, diagnoses, and treatment-related information.
5. **Visualize insights:** Use appropriate charts and summaries to communicate patterns clearly.
6. **Interpret findings:** Discuss what the analysis suggests, along with its limitations and potential business relevance.

## Planned Analysis

The main areas of investigation are:

| Analysis Area | Key Questions |
|---|---|
| Readmission patterns | How are encounters distributed across the recorded readmission categories? |
| Patient demographics | How do readmission patterns vary across age groups and gender? |
| Hospital utilization | Are length of stay and previous inpatient visits associated with readmission outcomes? |
| Diagnoses and treatment | What patterns appear across diagnosis, procedure, and medication-related fields? |
| Comparative analysis | Which patient or encounter groups show different readmission patterns? |
| Data visualization | How can these findings be communicated clearly to support decision-making? |

## Expected Business Value

The project aims to demonstrate how healthcare data can be used to:

- Identify patient and encounter groups that may warrant further investigation.
- Understand patterns in hospital utilization and readmission outcomes.
- Support discussions around discharge planning, follow-up care, and resource allocation.
- Present complex healthcare data through clear, accessible visualizations.
- Demonstrate a structured, evidence-based approach to solving a real-world analytical problem.

These are intended applications of the analysis, not claims that the dataset alone can establish the causes of readmission or measure overall care quality.

## Repository Structure

The repository will be organized as follows:

```text
Healthcare-Analytics/
│
├── data/
│   └── diabetic_data.csv
│
├── Healthcare_Analytics_Phase1.ipynb
│
├── Healthcare_Analytics_SRS.docx
│
└── README.md
```

- `data/diabetic_data.csv` – Original dataset used for the project.
- `Healthcare_Analytics_Phase1.ipynb` – Project overview, business problem, objectives, dataset inspection, planned analysis, and scope.
- `Healthcare_Analytics_SRS.docx` – Software Requirements Specification documenting the project requirements.
- `README.md` – Project overview and documentation.

## Scope and Limitations

- The dataset covers historical hospital encounters from **1999 to 2008**; findings may not reflect current healthcare practices.
- The analysis is based on the variables available in the dataset.
- Multiple encounters may belong to the same patient.
- Associations between patient or encounter characteristics and readmission do not establish causation.
- Readmission status alone is not a complete measure of healthcare quality.
- The project focuses on analytical insights and does not provide medical advice or individual patient recommendations.

## Project Status

**Phase 1 – Project Proposal and Initial Dataset Inspection**

The project scope, business problem, objectives, dataset requirements, and planned analysis are defined. The dataset has been loaded and its structure inspected.

Detailed exploratory analysis, visualizations, and evidence-based findings will be documented in subsequent phases.


This project brings together healthcare data and analytical thinking to explore a meaningful real-world problem. It emphasizes structured problem definition, data understanding, reproducible analysis, responsible interpretation, and clear communication of insights.

The objective is not simply to analyze a dataset, but to demonstrate how data analysis can help people ask better questions, understand patterns, and make more informed decisions.

