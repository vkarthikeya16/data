# Diabetic Retinopathy Dataset

Fundus images for automated diabetic retinopathy classification.

## Student Information

- **Name**: Karthikeya Vaitla
- **Email**: vaitlak@roehampton.ac.uk
- **Course**: Applications of Data Science
- **University**: University of Roehampton
- **Date**: December 2025

## Dataset Statistics

| Class | Images | Size | Percentage |
|-------|--------|------|------------|
| Healthy (No DR signs) | 187 | 73.9 MB | 24.7% |
| DR (DR signs present) | 570 | 306.8 MB | 75.3% |
| **Total** | **757** | **380.8 MB** | **100%** |

## Repository Structure

```
data/
├── images/
│   ├── Healthy/              # 187 fundus images
│   └── DR/                   # 570 fundus images
├── Annotations of the classifications.xlsx
├── file_manifest.txt        # Complete file listing
└── README.md                # This file
```

## Classification Criteria

- **Healthy**: Images with "No DR signs" annotation
- **DR**: Images with diabetic retinopathy signs

## Usage with MATLAB Pipeline

This dataset integrates with the cloud-enabled classification pipeline:

```matlab
% Configure cloud loading
cloudConfig.github.username = 'YOUR_USERNAME';
cloudConfig.github.repository = 'diabetic-retinopathy-dataset';

% Run pipeline - images download automatically
main_pipeline_cloud_enabled
```

## Machine Learning Approach

Classical ML algorithms:
- k-Nearest Neighbors (k-NN)
- Decision Trees
- Logistic Regression
- Support Vector Machines (SVM)
- Naive Bayes

Feature extraction:
- Gabor filters
- Local Binary Patterns (LBP)
- Histogram of Oriented Gradients (HOG)

## License

Academic use only - University of Roehampton coursework.
