# Dentora-AI

AI-powered dental radiograph analysis for tooth detection, numbering, and future clinical decision support.

Dentora-AI is an early-stage research and engineering project focused on building a modular pipeline for dental X-ray analysis using computer vision and deep learning. The goal is to create a robust foundation for analyzing panoramic dental radiographs, localizing teeth, assigning standard dental numbering, and eventually extending the system to support broader clinical findings.

## Overview

Dental imaging is a core part of modern dentistry, and AI-driven analysis can help streamline workflows, improve consistency, and support clinical decision-making. Dentora-AI aims to explore the development of reliable and interpretable models for:

- tooth detection
- tooth localization
- FDI tooth numbering
- segmentation-based analysis
- future dental finding detection

The repository is intentionally structured to support research-first development, reproducible experiments, and long-term extensibility as more datasets, models, and evaluation pipelines are added.

## Why Dentora-AI?

The project addresses a practical and technically rich problem in dental imaging:

- large amounts of radiographic data are produced in routine dental care
- annotation and labeling can be time-consuming and expensive
- automated analysis can support diagnostics, treatment planning, and workflow optimization
- standardized outputs are essential for research and deployment

By combining Python-based ML tooling, computer vision techniques, and a modular architecture, Dentora-AI provides a foundation for building research-grade dental AI systems.

## Current Project Status

This repository is currently in an early-stage research and development phase. The core focus is on project setup, reproducible experimentation, and developing a clean foundation for future model training and evaluation.

The project is expected to evolve in phases:

1. dataset review and validation
2. baseline model development
3. tooth detection and localization
4. tooth numbering and structured outputs
5. segmentation and advanced research tasks
6. deployment and UI-based demonstration

## Core Features (Planned and In Progress)

- Tooth detection on panoramic dental X-rays
- FDI tooth numbering using clinically accepted conventions
- Instance segmentation for individual teeth
- Detection of common dental findings when suitable datasets are available
- Structured outputs for model predictions, confidence scores, and metadata
- Visualization overlays for detected regions and numbering
- Extensible architecture for future research and experiment tracking

## Technology Stack

- Python
- PyTorch
- OpenCV
- FastAPI
- Pydantic
- Streamlit
- Docker
- pytest
- NumPy
- scikit-learn (likely for evaluation workflows)

The stack may expand or change as the project matures and specific research tasks become more defined.

## Repository Structure

```text
Dentora-AI/
├── app/
│   └── __init__.py
├── src/
│   └── __init__.py
├── .gitignore
├── README.md
├── requirements.txt
└── ...
```

### Directory Notes

- app/: application-level package entry points and service layers
- src/: core source code, model logic, utilities, and training-related modules
- requirements.txt: project dependencies
- README.md: project overview and setup instructions

## Getting Started

### Prerequisites

Before starting, make sure you have:

- Python 3.10 or newer
- pip
- virtual environment support
- Git

### Clone the Repository

```bash
git clone https://github.com/HosseinHeydari2004/Dentora-AI.git
cd Dentora-AI
```

### Create a Virtual Environment

```bash
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
# or
.venv\Scripts\activate     # Windows
```

### Install Dependencies

The dependency list is still being finalized as the project evolves. In a development environment, install the core packages needed for image processing and ML workflows:

```bash
pip install --upgrade pip
pip install torch torchvision opencv-python-headless numpy pandas matplotlib
pip install fastapi uvicorn pydantic streamlit pytest
```

If the project introduces a pinned requirements file later, use:

```bash
pip install -r requirements.txt
```

## Recommended Project Workflow

A typical research workflow for this project is:

1. collect and inspect dental X-ray datasets
2. clean and preprocess images
3. annotate or validate labels
4. build baseline detection models
5. evaluate model performance using relevant metrics
6. visualize predictions and error cases
7. iterate on model architecture and preprocessing

## Data and Evaluation Strategy

The project is intended to use publicly available dental datasets when licensing and access terms permit. Data preparation should follow careful practices, including:

- patient-level splitting to avoid leakage
- documentation of annotation sources
- validation against dental domain requirements
- clear tracking of dataset version and metadata

Evaluation should be task-appropriate and may include metrics such as:

- precision and recall
- mAP for detection tasks
- segmentation IoU
- clinical validation reviews where applicable

## Example Target Use Cases

- dental clinic workflow support
- research on automated tooth localization
- AI-assisted diagnostic pipelines
- educational tooling for image analysis
- dataset benchmarking and model comparison

## Roadmap

### Phase 1: Foundation
- repository structure and project documentation
- environment setup and dependency tracking
- data exploration and preprocessing notebooks or scripts

### Phase 2: Baselines
- tooth localization models
- config-driven experiment setup
- standard evaluation pipeline

### Phase 3: Clinical Tasks
- FDI numbering
- structured outputs and predictions
- visualization tools

### Phase 4: Expansion
- segmentation and advanced findings
- API/service layer
- UI prototype or demo application

## Contributing

Contributions are welcome as the project develops. If you would like to contribute:

1. fork the repository
2. create a feature branch
3. implement your changes with documentation
4. validate the relevant workflow or tests
5. open a pull request with a clear explanation

Suggested areas for contribution:

- dataset preprocessing utilities
- model training scripts
- evaluation metrics
- visualization tools
- API or web interface components
- documentation improvements

## Testing

The project is still in its early stages, and testing practices will mature over time. A basic test setup is recommended for:

- preprocessing functions
- dataset validation utilities
- model output parsing
- metric computations

Example:

```bash
pytest
```

## License

This project is currently in an early development stage, and licensing details should be reviewed before broader use or distribution. If you are using external datasets, check the dataset-specific terms and ensure compliance with all relevant licensing requirements.

## Acknowledgments

This project is inspired by the intersection of medical imaging, computer vision, and applied AI research. Future acknowledgments may include specific datasets, open-source libraries, and research collaborators.

## Contact

For questions, collaboration ideas, or project discussions, please reach out through the repository's GitHub issues or by contacting the project maintainer.

---

Built for dental AI research, experimentation, and future clinical tooling.
