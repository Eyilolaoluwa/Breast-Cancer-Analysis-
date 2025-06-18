#  Breast Cancer Diagnosis Classification Using k-NN in R

This project applies the **k-Nearest Neighbors (k-NN)** algorithm to classify tumors as **Benign** or **Malignant** using the **Wisconsin Breast Cancer Diagnostic** dataset.

---

##  Dataset

- **Source**: `wisc_bc_data.csv`
- **Instances**: 569
- **Features**: 30 numeric features derived from images of breast masses
- **Target Variable**: `diagnosis` (B = Benign, M = Malignant)

---

## Step 1: Exploring and Preparing the Data

- **Load the dataset**
```r
wbcd <- read.csv("wisc_bc_data.csv", stringsAsFactors = FALSE)
wbcd <- wbcd[-1]
