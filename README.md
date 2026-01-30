# Bone Health Screening Gaps – NHANES 2005–2006 (Public Demo)

This repository contains a public, reproducible analysis examining gaps in age-based osteoporosis screening using data from the **NHANES 2005–2006** cohort. The analysis focuses on identifying individuals at high bone-health risk who are not captured by current age-based screening criteria.

All analyses are conducted for demonstration and portfolio purposes only.

---

## What this analysis shows

- The proportion of the population that is **screening-eligible** under current age-based guidelines  
- The proportion classified as **high bone-health risk** based on bone density and clinical/lifestyle proxies  
- The size and characteristics of the **missed high-risk population** (high risk but not screening-eligible)  
- How alternative screening scenarios (age expansion and risk-proxy triggers) reduce missed high-risk cases  
- Segment-level patterns by age, sex, and race/ethnicity, including equity guardrails  

---

## Key concepts

The analysis focuses on three overlapping groups:

1. **Screening-eligible individuals** (based on age and sex criteria)
2. **High bone-health risk individuals** (based on DXA lumbar spine T-scores and clinical/lifestyle factors)
3. **Missed high-risk individuals**, defined as those at high risk who are not screening-eligible

The primary objective is to quantify and illustrate the size of the missed high-risk group and explore how alternative screening logic could reduce this gap.

---

## Data sources

Publicly available data from the **NHANES 2005–2006** cycle were used, including:

- Demographics  
- Body measurements  
- Dual-energy X-ray absorptiometry (DXA)  
- Osteoporosis questionnaire  
- Smoking behavior  
- Physical activity  

All data were merged using the NHANES respondent identifier (`SEQN`).

---

## Methods (high level)

- Relevant variables were selected from each dataset based on clinical relevance  
- Lumbar spine T-scores were used to classify bone density status  
- High bone-risk status was defined using a combination of DXA results and risk proxies  
- Missing data were assessed and handled conservatively to avoid inflating risk estimates  
- Multiple screening scenarios were evaluated to estimate potential reductions in missed high-risk cases  
- Results were summarized using tables and interpretable visualizations  

---

## Important notes

- This analysis uses **real NHANES data**, but all interpretations are for **demonstration purposes only**  
- No clinical decisions should be made based on this analysis  
- Screening rules and thresholds are simplified proxies, not clinical recommendations  
- Minor differences from published prevalence estimates may occur due to analytic choices and exclusions  

---

## How to view the report

The full rendered report is available via **GitHub Pages**:

➡️ *[Insert GitHub Pages link here]*

---

## R packages used

The analysis was conducted in R using the following packages:

- **Data manipulation & pipelines**  
  - magrittr  
  - tidyverse  
  - dplyr  
  - tibble  
  - janitor  

- **Data import & export**  
  - haven  
  - readxl  
  - writexl  

- **Analysis & utilities**  
  - psych  
  - scales  

- **Visualisation & reporting**  
  - ggplot2  
  - knitr  
  - kableExtra  

---

## License

This project is provided for educational and demonstration purposes only.
