# ppg-resources (Photoplethysmography)

A curated collection of high-quality libraries, datasets, research papers, and other resources for Photoplethysmography (PPG) analysis, with a focus on embedded PPG solutions for edge devices. This repository is designed to be a comprehensive and well-organized guide for researchers and developers working in the field of PPG, particularly those building efficient, real-time applications on resource-constrained hardware.

## Papers 

### Biomarker detection
 #### Blood pressure
 
 #### Diabetes
 - 2025 [IoT and cloud‑based non‑invasive diabetes detection system from photoplethysmogram](https://www.researchgate.net/publication/391736513_IoT_and_cloud-based_non-invasive_diabetes_detection_system_from_photoplethysmogram)
 
---
### Motion/Noise Artifacts detection
 #### Statistical approach
 - 2011 [Statistical Approach for the Detection of Motion/Noise Artifacts in Photoplethysmogram](https://pubmed.ncbi.nlm.nih.gov/22255454/)

---
### Signal quality assessment

- 2012 [Photoplethysmogram signal quality estimation using repeated Gaussian filters and cross-correlation](https://iopscience.iop.org/article/10.1088/0967-3334/33/10/1617)
- 2015 [Signal-quality indices for the electrocardiogram and photoplethysmogram: derivation and applications to wireless monitoring](https://pubmed.ncbi.nlm.nih.gov/25069129/)
- 2022 [Wrist Photoplethysmography Signal Quality Assessment for Reliable Heart Rate Estimate and Morphological Analysis](https://pubmed.ncbi.nlm.nih.gov/35957395/)


## Datasets

### [PPG-BP dataset](https://figshare.com/articles/dataset/PPG-BP_Database_zip/5459299)
- **Subjects:** 219 (age 20–89)  
- **Segments:** 657 PPG recordings
- **Data**: One-channel fingertip PPG, three measurements of 2.1 seconds per subject. Each of the three segments has a skewness SQI assigned.PPG measurements are accompanied by systolic/distolic pressure, HR and medical record label (diabetes, cardiovascular disease)
- **Conditions included:** Hypertension, diabetes, cardiovascular disease  
- **Collection:** Controlled experimental environment  
- **License:** CC0 (public domain)  
- **Purpose:** Study relationship between PPG and blood pressure; useful for anomaly detection (pathological vs. “normal” PPG patterns) and cardiovascular screening
  
### [Mazandaran](https://data.mendeley.com/datasets/37pm7jk7jn/2)

- **Subjects:** 23 individuals  
- **Segments:** 67 fingertip PPG recordings  
- **Data:** One-channel green LED PPG (≈550 nm), sampled at 2,175 Hz. Each sample is paired with demographic information (age, gender, weight, height) and invasive blood glucose measurements. Archive includes raw `.mat` signals, metadata labels, and signal plots.  
- **Conditions included:** Variation in blood glucose levels (hypo-, normo-, hyper-glycemia); no motion artifact scenarios.  
- **Collection:** Controlled laboratory environment, fingertip sensor with amplification + filtering, digitized via MCU ADC.  
- **License:** CC BY 4.0 (open access)  
- **Purpose:** Designed for non-invasive blood glucose estimation from PPG; useful for studying **physiological anomaly detection** (glucose-related signal variation), but not suited for motion/noise anomaly detection or multi-wavelength comparisons.  

### [Cuff-Less Blood Pressure Estimation](https://archive.ics.uci.edu/dataset/340/cuff+less+blood+pressure+estimation)

- **Subjects:** Not specified (derived from PhysioNet recordings)  
- **Segments:** 12,000 signal segments  
- **Data:**  
  - Three-channel physiological signals per segment:
    - **PPG** (photoplethysmogram) from the fingertip  
    - **ABP** (arterial blood pressure) in mmHg (invasive)  
    - **ECG** (Lead II)  
  - Sampling rate: 125 Hz for all channels  
  - Format: MATLAB v7.3 `.mat` files (HDF5-compatible)  
- **Conditions included:**  
  - Cleaned, high-quality segments suitable for model training  
  - No annotations for motion artifacts or physiological state variations  
- **Collection:**  
  - Signals originally sourced from PhysioNet databases  
  - Preprocessed, validated, and labeled by dataset creators (Kachuee et al., 2015)  
- **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (open access, attribution required)  
- **Purpose:**  
  - Designed for non-invasive, cuff-less blood pressure estimation using features like pulse transit time  
  - Ideal for signal processing, machine learning regression models  
  - Not suitable for:
    - Motion/noise artifact detection  
    - Classification tasks involving medical conditions  
