# Collaborative_Filtering_for_Implicit_Feedback_Datasets
Project for the Data Mining course – University of Verona

# Collaborative Filtering for Implicit Feedback Datasets  

Project developed for the **Data Mining** course at the University of Verona.  
The work is inspired by the paper *"Collaborative Filtering for Implicit Feedback Datasets"* (Hu, Koren, Volinsky, 2008).  

---

## Repository Structure
- **notebooks/**  
  Jupyter Notebook with the full implementation, including:
  - Baselines: *Popularity*, *Item–Item CF*  
  - Implicit ALS with linear and log confidence  
  - Evaluation metrics: *Recall@K*, *MAP@K*, *Expected Percentile Ranking (EPR)*  

- **data/**  
  Reduced version of the **Last.fm 1K dataset**  
  - `profiles_first500.csv`  
  - `listens_first500_CAP.csv`  
  (subset generated for feasibility reasons, ~500 users and ~2M interactions)

- **report/**  
  Final report in PDF/LaTeX format, describing methodology, experiments, results, and discussion.  

---

## Project Goals
- Re-implement and test the ALS model for implicit feedback.  
- Benchmark against simpler baselines (*Popularity*, *Item–Item*).  
- Analyze sensitivity to hyperparameters (*factors, α, λ*).  
- Discuss strengths, limitations, and possible improvements (e.g., popularity bias, parameter tuning).  

---

## Dataset
The experiments are based on a **subset of the Last.fm 1K Dataset (2009)**.  
A reduced version was generated for this project (first ~500 users, ~2 million interactions) to ensure computational feasibility.  
