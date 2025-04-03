# Medical-ReportGeneration

Dataset: https://www.kaggle.com/datasets/raddar/chest-xrays-indiana-university

About Dataset
Open access chest X-ray collection from Indiana University
Original source: https://openi.nlm.nih.gov/

Original images were downloaded in raw DICOM standard. Each image was converted to png using some post-processing:

top/bottom 0.5% DICOM pixel values were clipped (to eliminate very dark or very bright pixel outliers)
DICOM pixel values scaled linearly to fit into 0-255 range
resized to 2048 on shorter side (to fit in Kaggle dataset limits)
Metadata downloaded using available API (https://openi.nlm.nih.gov/services#searchAPIUsingGET)

Each image classified manually into frontal and lateral chest X-ray categories.
