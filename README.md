# Alzheimer-s-Disease-MRI-Feature-Extraction-Visualization

## Executive Summary

This project focuses on transforming raw Alzheimer’s Disease MRI brain scan images into a structured and analyzable dataset. Using Python, key radiological features such as pixel intensity, entropy, and structural clarity were extracted from thousands of MRI scans and converted into a clean CSV file. The resulting dataset was visualized in Power BI to uncover insights into disease patterns, severity levels, and structural brain changes across dementia categories.
This workflow provides a reproducible pipeline that bridges medical imaging, data engineering, and business intelligence.

The raw file where the images of the MRI Scan was sourced from- https://www.kaggle.com/datasets/aryansinghal10/alzheimers-multiclass-dataset-equal-and-augmented

## Business Problem

Hospitals and research centers often store MRI scans as raw image files, making it difficult for clinicians and data teams to:
- Compare brain scans using measurable metrics
- Detect early structural changes associated with Alzheimer’s
- Build dashboards for medical insights
- Integrate imaging data into predictive models
- Raw images are not directly analyzable.
  
There is a need for a data engineering pipeline that converts MRI images into quantifiable metrics that can support diagnosis, monitoring, and research.

## Methodology
1. Data Ingestion
   
 Loaded 4 MRI scan categories:
- MildDemented, ModerateDemented, VeryMildDemented, NonDemented
- Handled hundreds of PNG/JPG MRI slices.

2. Image Processing in Python
   
Using PIL, NumPy, and scikit-image, the following features were extracted:
- Feature	Meaning
- Mean Pixel Intensity	Average brightness of brain tissue
- Standard Deviation	Variability in brightness (structural variation)
- Shannon Entropy	Complexity / disorder level in the scan
- Edge Density (Sobel Filter)	Structural clarity & boundaries
- Center Brightness	Measures atrophy or tissue loss in the brain center
- Is Augmented	Identifies artificially created training images
  
4. Data Transformation
- Standardized filenames
- Assigned labels
- Stored extracted features in a structured CSV file

6. Visualization in Power BI
- Created an interactive dashboard showcasing:
- Disease progression metrics
- Entropy and brightness trends
- Top healthy vs diseased scans
- Structural clarity comparisons
- Pixel intensity statistics
- Class distribution analysis

## Skills Demonstrated
- Programming & Data Engineering
- Python scripting
- File system automation
-  Image processing (PIL, skimage)
- Feature engineering
- Data transformation (NumPy, Pandas)
- Data Visualization
- Power BI dashboard creation
- KPI cards, bar charts, donut charts
- Visual storytelling with medical imaging
- Machine Learning Readiness
- Feature extraction for classification models
- Clean structured dataset suitable for ML pipelines

### Software & Tools
Python
NumPy, Pandas
PIL, scikit-image
tqdm
Power BI Desktop
GitHub

## Results & Insights

Using automated MRI feature extraction:

✔ Structured CSV Dataset Generated

Thousands of MRI scans processed

Extracted 6+ numerical features per image

Dataset now ready for ML classification or EDA

✔ Key Visual Insights in Power BI

NonDemented patients show higher structural clarity

ModerateDemented scans show lower brightness and higher disorder

Center brightness trends help identify early-stage tissue loss

Entropy levels reveal clear separation between healthy and diseased groups

✔ Dashboard Enables

Quick review of disease severity

Comparison between dementia categories

Medical image analytics in business-friendly visuals

📌 Business Requirements Addressed

Requirement	How This Project Solves It:
- Convert MRI images into analyzable data	Python pipeline extracts structured features
- Identify brain structural differences	Extracted radiological metrics highlight patterns
- Generate diagnostic insights	Power BI KPIs show progression trends
- Enable integration into ML models	Output CSV is clean and ML-ready
- Support medical decision-making	Visual summaries provide interpretable metrics

🚀 Next Steps
1. Build a Machine Learning Model

- Train a classifier (Random Forest, XGBoost, CNN)
- Predict dementia category based on extracted MRI features

2. Deep Learning Embeddings

Use a pre-trained CNN (ResNet, VGG16) to extract deeper image representations.

3. Cloud Deployment

- Deploy the pipeline on Azure/AWS
- Store MRI metrics in cloud databases
- Serve dashboards via Power BI Service

4. Add Clinical Metadata

 Combine MRI features with:
- Age
- Gender
- Cognitive scores

5. Real-Time Inference

Build a UI where clinicians upload MRI scans and get:

- Feature summary
- Risk level score
- Visual explanation

<img width="591" height="325" alt="image" src="https://github.com/user-attachments/assets/c64b9310-b096-470f-89ad-0c26c6ef57ff" />

