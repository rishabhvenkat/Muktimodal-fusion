# Stroke Outcome Prediction Using Multimodal Fusion

Predict stroke outcomes in acute ischemic patients using clinical and neuroimaging data.

## Data
- **Patients:** 313 from the 1000plus study  
- **Clinical predictors (7):** NIHSS, thrombolysis, cardiac history, gender, diabetes, hypercholesterolemia, age  
- **Neuroimaging:** 3D TOF-MRA scans (156x192x64 voxels)  
- **Output:** 3-month mRS score (Good: ≤2, Bad: ≥3)  
> Data not publicly available due to privacy restrictions

## Models
- **MLP:** Clinical data  
- **CNN:** 3D neuroimaging  
- **Multimodal Fusion:** Combines clinical + imaging via extracted features or end-to-end training

## Training & Evaluation
- **Loss:** Binary cross-entropy  
- **Optimizer:** Adam  
- **Metrics:** AUC over multiple splits and runs  
- **Significance:** Wilcoxon signed-rank test to compare multimodal vs. MLP  

## License
MIT
