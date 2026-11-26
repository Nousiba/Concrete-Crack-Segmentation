# Dataset Information

## Dataset Overview
- **Name:** Concrete Crack Segmentation Dataset
- **Author:** Çağlar Fırat Özgenel
- **Source:** Mendeley Data
- **Publication Date:** April 3, 2019
- **Version:** 1
- **DOI:** 10.17632/jwsn7tfbrp.1
- **URL:** https://data.mendeley.com/datasets/jwsn7tfbrp/1

## Dataset Description
The dataset contains real-world concrete surface images and corresponding pixel-level ground truth masks. The original dataset description reports 458 high-resolution images designed for concrete crack segmentation.

## Dataset Structure
- **rgb:** Original concrete surface images.
- **BW:** Ground truth crack masks.

## Initial Dataset Inspection
- RGB images: 445.
- BW masks: 458.
- Matching image-mask pairs: 445.
- Images without masks: 0.
- Masks without images: 13.

Images and masks will be matched by filename. Invalid and unmatched files will be excluded.

## Image Specifications
- Color format: RGB.
- Ground truth format: Crack masks.
- Processing resolution: Maximum side of 1024 pixels, preserving aspect ratio.
- Data type: uint8.
- Bit depth: 8 bits per channel.
- Intensity range: 0–255.
- Binary mask values: 0 and 1 after preprocessing.

## Dataset Challenges
- Low contrast.
- Uneven illumination.
- Complex surface textures.
- Thin and irregular cracks.
- Potential image noise.
- Disconnected crack regions.

## Dataset Requirements Verification
- Real-world images: Available.
- Pixel-level ground truth: Available.
- Minimum dataset size: Verified (445 matching image-mask pairs).
- Academic use licence: Verified (CC BY 4.0).
- Google Colab compatibility: Successfully tested.

## Data Preparation
- Match images with corresponding ground truth masks.
- Remove invalid and unmatched files.
- Verify image dimensions and data types.
- Standardize image loading and intensity ranges.
- Convert RGB images to grayscale when required.
- Use fixed random seeds for reproducibility.

## Data Splitting
- **Development Set:** 70%.
- **Test Set:** 30%.

The development set will be used for experimentation and parameter tuning. The test set will be reserved exclusively for final evaluation.

## Ground Truth
Ground truth masks identify crack regions as foreground pixels and non-crack regions as background pixels.

## Controlled Degradation
- Gaussian noise.
- Salt-and-pepper noise.

Controlled noise levels and fixed random seeds will be used for reproducible restoration experiments.

## Evaluation Metrics
- **IoU:** Primary segmentation evaluation metric.
- **MSE:** Image restoration error measurement.
- **PSNR:** Image restoration quality measurement.

## Dataset Download Instructions
1. Open the dataset URL.
2. Download and extract the dataset archive.
3. Locate the rgb and BW folders.
4. Verify image-mask correspondence.
5. Prepare the development and test sets.

## Dataset Storage
The dataset will be accessed through Google Drive and Google Colab. Large raw image files will not be uploaded to GitHub.

## Current Status
Dataset preparation, image-mask pairing, image analysis, metric testing, and baseline experiments have been completed successfully. A total of 445 matching image-mask pairs were identified. Dataset licence has been verified as CC BY 4.0.
