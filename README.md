# Collaborative_Filtering_for_Implicit_Feedback_Datasets  

Project developed for the **Mining Massive Datasets** course at the University of Verona.  
The work is inspired by the paper *"Collaborative Filtering for Implicit Feedback Datasets"* (Hu, Koren, Volinsky, 2008).  

---

## Repository Structure
- **Collaborative Filtering for Implicit Feedback.pdf** → Original paper (Hu, Koren, Volinsky, 2008).  
- **Dataset_Reduction.ipynb** → Jupyter Notebook for the creation of the Last.fm subset.  
- **Implicit_Feedback_Report.pdf** → Final report (PDF/LaTeX) with methodology, experiments, results, and discussion.  
- **Official_Implicit_Feedback.ipynb** → Jupyter Notebook with the full implementation, including:  
  - Baselines: *Popularity*, *Item–Item CF*  
  - Implicit ALS with linear and log confidence  
  - Evaluation metrics: *Recall@K*, *MAP@K*, *Expected Percentile Ranking (EPR)*  

---

## Project Goals
- Re-implement and test the ALS model for implicit feedback.  
- Benchmark against simpler baselines (*Popularity*, *Item–Item*).  
- Analyze sensitivity to hyperparameters (*factors, α, λ*).  
- Discuss strengths, limitations, and possible improvements (e.g., popularity bias, parameter tuning).  

---

## Dataset
The experiments are based on the **subset of the Last.fm 1K Dataset (2009)**.  
The original dataset was collected from the Last.fm API (`user.getRecentTracks`) and contains complete listening histories for ~1,000 users until May 5, 2009.

-  Download: [Last.fm 1K Dataset](http://ocelma.net/MusicRecommendationDataset/lastfm-1K.html)  
-  Contents:
  - `userid-timestamp-artid-artname-traid-traname.tsv` → listening events (user, timestamp, artist, track)
  - `userid-profile.tsv` → user profile information (gender, age, country, signup date)
  - `README.txt`→ Full dataset description

For this project, a **reduced version** was generated (~500 users, ~2M interactions) to ensure computational feasibility.

---

