# Real-World Data Analytics Demo (SQL + Python, OMOP-CDM)

This repository demonstrates how to analyze synthetic **electronic medical records (EMR)** using the **OMOP Common Data Model (CDM)** framework.  

---

## Key Features

- **SQL for cohort building**
  - Example queries for patient selection, condition prevalence, and comorbidity co-occurrence.
- **Python for predictive modeling**
  - Logistic regression applied to respiratory outcomes.
- **OMOP-CDM structure**
  - `person` table (demographics: age, sex, race).  
  - `condition_occurrence` table (SNOMED-coded conditions).  
- **Clinical terminologies**
  - Uses OMOP `condition_concept_id`s mapped to SNOMED CT, compatible with ICD.  
- **Visualization**
  - Co-occurrence heatmaps, cohort characterization plots, feature importance analysis.  

---

## Relevance to RWE

This demo showcases the core workflow used in RWE analytics:  

- Cohort definition
- Comorbidity analysis
- Predictive modeling
- Visualization & interpretation

Even though data are synthetic, the methods are directly transferable to EMR and claims data.  

---

## Quick start

```bash
git clone https://github.com/ivkarla/rwd-sql-python-demo
cd rwd-sql-python-demo
conda create -n rwd-demo python=3.10
conda activate rwd-demo
pip install -e .