# Concrete Crack Segmentation Using Classical Digital Image Processing

## Course Information

University: Alamein International University

Faculty: Computer Science and Engineering

Course: Digital Image Processing

Course Code: CSE281

## Team Members and Roles

**Nousiba Adel**  
Tech Lead & Data and Baseline Engineer

**Nada Elshahat**  
Enhancement Engineer

**Maryam Yasser**  
Restoration & Frequency Engineer

**Mariam Emad**  
Segmentation Engineer

**Yasmin Salah**  
Morphology & Evaluation Engineer

## Project Overview

This project aims to develop a classical digital image processing pipeline for detecting and segmenting cracks in concrete surfaces and estimating the percentage of cracked surface area.

## Problem Statement

Manual inspection of concrete cracks can be time-consuming and susceptible to human error. Automatic crack detection is challenging due to low contrast, uneven illumination, noise, irregular crack shapes, and complex surface textures.

The proposed system applies classical digital image processing techniques to identify cracks, generate binary segmentation masks, and measure the affected surface area.

## Target Users

- Civil engineers.
- Structural inspectors.
- Infrastructure maintenance teams.

## Cost of Errors

Missing cracks may result in overlooking potential structural damage, while false detections may lead to unnecessary inspections and maintenance costs.

## Project Objectives

- Detect cracks in concrete surface images.
- Improve image contrast and visibility.
- Reduce image noise.
- Separate cracks from the background.
- Generate binary crack masks.
- Refine segmentation using morphological operations.
- Calculate the percentage of cracked surface area.
- Compare different image processing techniques.
- Evaluate performance against ground truth masks.

## Dataset Information

Dataset Name: Concrete Crack Segmentation Dataset

Author: Çağlar Fırat Özgenel

Source: Mendeley Data

Dataset URL: https://data.mendeley.com/datasets/jwsn7tfbrp/1

DOI: 10.17632/jwsn7tfbrp.1

The dataset contains real-world concrete surface images and corresponding pixel-level ground truth masks.

## Input

RGB concrete surface images.

Image dimensions, bit depth, data type, and intensity range will be verified during dataset analysis.

## Output

- Binary crack segmentation masks.
- Crack area in pixels.
- Crack area percentage.

## Primary Evaluation Metric

Intersection over Union (IoU).

IoU measures the overlap between the predicted crack mask and the ground truth mask relative to their combined area.

IoU = Intersection Area / Union Area

IoU is selected because it accounts for both missed cracks and incorrectly detected regions.

## Secondary Evaluation Metrics

- Mean Squared Error (MSE).
- Peak Signal-to-Noise Ratio (PSNR).
- Processing time.

MSE and PSNR will be used for image restoration experiments.

## Proposed Methodology

1. Dataset preparation.
2. Image analysis.
3. Baseline implementation.
4. Image enhancement.
5. Image restoration.
6. Frequency-domain processing.
7. Image segmentation.
8. Morphological refinement.
9. Crack area measurement.
10. Performance evaluation.

## Baseline Methods

**Baseline 1:** Fixed global thresholding with a threshold value of 127.

**Baseline 2:** Otsu thresholding followed by morphological opening using a 3 × 3 structuring element.

## Data Splitting

- Development Set: 70%.
- Test Set: 30%.

The development set will be used for experimentation and parameter tuning. The test set will be reserved exclusively for final evaluation.

## Project Scope

The project relies exclusively on classical digital image processing techniques without training machine learning or deep learning models.

## Tools and Technologies

- Python
- NumPy
- OpenCV
- SciPy
- scikit-image
- Matplotlib
- Pandas
- Google Colab
- GitHub

## Milestone 1: Project Preparation

- Problem selection.
- Dataset selection and verification.
- Problem formulation.
- Primary metric selection.
- Team role assignment.
- GitHub repository preparation
