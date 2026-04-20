

# Heart Disease Prediction Using Machine Learning

Using the UCI Cleveland Heart Disease dataset  
<https://archive.ics.uci.edu/dataset/45/heart+disease>

Comparative machine‑learning study on the UCI Cleveland Heart Disease dataset, evaluating **6 classifiers** with hyperparameter tuning and test‑set permutation importance to achieve **88.52% accuracy and 96.43%** sensitivity for binary heart‑disease prediction.
paste.txt
+1

***

## Project Overview

This project was developed as part of the **MSc Data Science Individual Project (7PAM2002)** at the **University of Hertfordshire** (Semester B, 2025/2026).

**Objective**

Develop and compare machine‑learning models for binary heart‑disease classification, optimise hyperparameters, and provide a reproducible, clinically interpretable feature‑importance analysis. 

**Key achievements**

- 88.52% test accuracy with **Random Forest** (best model) 
- 96.43% sensitivity (recall) – only 2 of 28 diseased patients missed on the test set 
- ROC‑AUC ≈ 0.95 – excellent discrimination between healthy and diseased patients 
- Systematic GridSearchCV hyperparameter tuning (930 model fits) and tuning ROI analysis 
- **Test‑set** permutation‑importance methodology to validate key risk factors (ca, cp, oldpeak) 
- Fully reproducible pipeline with fixed random seeds and documented notebook 

***

## Research Questions

**Primary research question**

> Can machine‑learning classification models accurately predict heart‑disease presence using clinical and demographic features, and which algorithms and features perform best? 

**Secondary questions**

1. Which clinical features are most predictive of heart disease? 
2. How do different machine‑learning algorithms compare in performance on this dataset?  
3. Does hyperparameter tuning significantly improve model performance, and for which models? 
4. Can the predictions be explained in clinically interpretable terms (e.g. via permutation importance and error analysis)? [

***

## Dataset

- **Source:** UCI Machine Learning Repository – Heart Disease dataset (Cleveland subset). 
- **URL:** <https://archive.ics.uci.edu/dataset/45/heart+disease>  
- **File used:** `processed.cleveland.data` (303 patients, 13 features + target) 
- **Task:** Binary classification – presence vs absence of heart disease (0 vs 1) 

**Key dataset citation (clinical study)**

Detrano, R., Janosi, A., Steinbrunn, W., Pfisterer, M., Schmid, J.J., Sandhu, S., Guppy, K.H., Lee, S. and Froelicher, V. (1989) ‘International application of a new probability algorithm for the diagnosis of coronary artery disease’, *The American Journal of Cardiology*, 64(5), pp. 304–310. 

**Repository citation**

Dua, D. and Graff, C. (2019) *UCI Machine Learning Repository: Heart Disease Data Set*. University of California, Irvine. Available at: https://archive.ics.uci.edu/dataset/45/heart+disease (Accessed: 20 April 2026). 

Because this is anonymised, publicly available data, the project is a secondary data analysis and complies with UH ethical guidance without requiring new human data collection. 

***

## Files in this Repository

- `Notebook (24071919) heart_disease_analysis.ipynb` – final Jupyter notebook with full pipeline (EDA, preprocessing, models, tuning, permutation importance, plots). 
- `images/` – folder containing all figures used in the notebook and Final Project Report (distributions, correlations, ROC curves, feature‑importance plots).  
- `requirements.txt` – Python dependencies needed to run the notebook.  
- `(24071919) heart_disease_analysis.pdf` – Final Project Report submitted for 7PAM2002-0206-2025, matching the code in this repository. 

***

## How to Run

1. Install Python and clone this repository.  
2. Create a virtual environment (optional) and install packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Download `processed.cleveland.data` from the UCI link above and place it next to `heart_disease_analysis.ipynb` (or update the data path in the first cell).  
4. Start Jupyter and open `Notebook (24071919) heart_disease_analysis.ipynb`:

   ```bash
   jupyter notebook
   ```

5. Run all cells in order to reproduce the results and figures reported in the Final Project Report. 

***

