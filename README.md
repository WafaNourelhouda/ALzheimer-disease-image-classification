# ALzheimer-disease-image-classification
classifying Alzheimer's disease from MRI images using pretrained models and custom CNN architectures.

# Thesis: Alzheimer's Early Stage Detection Using Deep Learning

## Problem and Solution

### Problem:
Alzheimer's disease is one of the leading causes of dementia, and early detection is crucial for improving treatment outcomes. However, diagnosing Alzheimer's in its early stages is challenging, especially using traditional clinical methods. MRI scans are a powerful tool for detecting brain abnormalities associated with Alzheimer's, but interpreting these images accurately requires advanced techniques.

### Solution:
In my thesis, I focused on leveraging deep learning models to detect Alzheimer's disease at an early stage by analyzing brain MRI scans. The goal was to compare the performance of several deep learning models in terms of accuracy, efficiency, and clinical applicability. I compared **custom CNN architectures** with **pretrained models** such as **EfficientNetB3** and **InceptionV3**. The models were trained and evaluated on a dataset of brain MRIs, and key performance metrics were analyzed to identify the most effective model for early Alzheimer's detection.

---

## Model Comparison

The following table summarizes the performance of the different models in terms of key metrics like validation accuracy, AUC (Area Under Curve), loss, F1 score, recall, precision, and OASIS test accuracy:

| **Model**          | **Val Acc** | **Acc**  | **AUC**  | **Loss**   | **F1**  | **Recall** | **Precision** | **OASIS Test Acc** |
|--------------------|-------------|----------|----------|------------|---------|------------|---------------|-------------------|
| **CNN 1**          | 0.93        | 0.849    | 0.87     | 1.1093     | 0.64    | 0.64       | 0.65          | 0.34              |
| **CNN 2**          | 0.95        | 0.69     | 0.89     | 2.2112     | 0.674   | 0.685      | 0.685         | 0.67              |
| **CNN 3**          | 0.9709      | 0.9050   | 0.9725   | 0.0998     | 0.87    | 0.905      | 0.91          | 0.88              |
| **CNN 4**          | 0.99        | 0.6787   | 0.86     | 0.0269     | 0.68    | 0.67       | 0.68          | 0.25              |
| **EfficientNetB3** | 0.9828      | 0.99     | 0.99     | 0.13       | 0.50    | 0.48       | 0.53          | 0.33              |
| **InceptionV3**    | 0.98        | 0.90     | 0.98     | 0.2596     | 0.90    | 0.86       | 0.873         | 31.50             |

---

## Best Model Summary

Based on the overall evaluation, the best performing models across various metrics are highlighted below:

| **Metric**        | **Best Model**      | **Value**      |
|-------------------|---------------------|----------------|
| **Validation Accuracy** | CNN 4            | 0.99           |
| **Accuracy**          | EfficientNetB3     | 0.99           |
| **AUC**               | EfficientNetB3     | 0.99           |
| **Loss**              | CNN 4              | 0.0269         |
| **F1 Score**          | InceptionV3        | 0.90           |
| **Recall**            | CNN 3              | 0.90           |
| **Precision**         | CNN 3              | 0.91           |
| **OASIS Test Accuracy** | CNN 3            | 0.88           |

---

## Conclusion:
This study demonstrated the comparative performance of custom CNN models and pretrained architectures in detecting Alzheimer's disease from MRI scans. The **CNN 4** model achieved the highest accuracy and lowest loss, making it a top choice for clinical application. However, **EfficientNetB3** and **InceptionV3** performed excellently in several metrics, proving the potential of transfer learning for medical image analysis. These findings highlight the importance of selecting the right model architecture based on specific business and clinical needs.

---
