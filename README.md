# Dental AI

**AI-Powered Dental X-ray Analysis Platform**

Dental AI is an AI engineering and research project focused on developing computer vision solutions for dental radiograph analysis. The project aims to build a modular platform for tooth detection, FDI tooth numbering, and future dental finding analysis.

## Overview

The project explores deep learning methods for analyzing dental X-ray images, with an emphasis on reliable image processing, structured model outputs, reproducible experiments, and extensible software architecture.

The initial development phase focuses on panoramic dental radiographs and the foundations required for accurate tooth localization and numbering.

## Planned Features

- **Tooth Detection:** Localize individual teeth in panoramic dental X-rays.
- **FDI Tooth Numbering:** Assign tooth numbers according to the FDI World Dental Federation notation.
- **Tooth Instance Segmentation:** Explore pixel-level segmentation of individual teeth.
- **Dental Finding Detection:** Investigate the detection of dental caries and periapical lesions when suitable annotated datasets are available.
- **Structured Results:** Generate machine-readable outputs with tooth locations, model confidence, and model version information.
- **Visualization:** Display predicted bounding boxes, tooth numbers, and other supported model outputs.
- **Extensible Architecture:** Provide a foundation for future research and integration of additional dental AI models.

*Planned features are subject to dataset availability, annotation quality, and experimental validation.*

## Technical Stack

- Python
- PyTorch
- OpenCV
- FastAPI
- Pydantic
- Streamlit
- Docker
- pytest

The technology stack may evolve as the project progresses.

## Project Goals

1. Develop reproducible baselines for dental computer vision tasks.
2. Evaluate model performance using task-appropriate metrics.
3. Investigate robustness across image quality variations and challenging cases.
4. Build a maintainable inference pipeline and an interactive demonstration.
5. Establish a foundation for future scientific research and clinician-assisted evaluation.

## Dataset and Evaluation

The project will use publicly available dental radiograph datasets where their access conditions and licensing permit.

Dataset selection, annotation quality, patient-level data splitting, and licensing requirements will be documented before model training. Evaluation will use appropriate metrics, including mAP for object detection and task-specific metrics for tooth numbering and segmentation.

## Project Status

**Status:** Early-stage research and development.

The initial phase focuses on problem definition, dataset validation, baseline development, and evaluation protocol design. Features will be marked as implemented only after they have been developed and tested.


## License

The project license and dataset-specific usage conditions will be specified after reviewing the applicable licensing requirements.

---

**Built with Python and Deep Learning.**
