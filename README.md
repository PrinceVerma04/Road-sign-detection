
<img width="791" height="298" alt="Screenshot from 2025-09-30 16-38-53" src="https://github.com/user-attachments/assets/befffae2-dc20-4682-a88d-bf5761c20b86" />
<img width="206" height="241" alt="Screenshot from 2025-09-30 16-31-32" src="https://github.com/user-attachments/assets/21b27954-9d1b-4a50-800a-fa95ec342f44" /><img width="372" height="242" alt="Screenshot from 2025-09-30 16-31-10" src="https://github.com/user-attachments/assets/f33b22f8-2581-4c03-bfe9-f17ce52e5082" />


# Road Sign Detection

A computer vision project for detecting and classifying road signs using deep learning. This project explores a dataset of road sign images with XML annotations in PASCAL VOC format and provides a foundation for building road sign detection models.

## Project Structure 
road-sign-detection/
├── data/ # Dataset directories

│ ├── raw/ # Raw dataset files

│ └── processed/ # Processed dataset files

├── models/ # Trained model files

├── src/ # Source code modules

│ ├── data_preprocessing.py

│ ├── model.py

│ └── utils.py

├── notebooks/ # Jupyter notebooks for exploration

├── config/ # Configuration files

├── scripts/ # Training and prediction scripts

├── requirements.txt # Python dependencies

└── README.md # Project documentation
<!-- <img width="378" height="224" alt="Screenshot from 2025-09-30 16-50-13" src="https://github.com/user-attachments/assets/74da03d5-7cdc-4bcc-934d-3e44dac66fb4" /> -->



## Dataset
Dataset Link:-https://www.kaggle.com/datasets/andrewmvd/road-sign-detection

The dataset contains 877 images of 4 distinct classes for the objective of road sign detection road sign images with corresponding XML annotations in PASCAL VOC format. The dataset structure includes:
- `images/` directory with PNG images
- `annotations/` directory with XML annotation file
Bounding box annotations are provided in the PASCAL VOC format.

The classes are:

Trafic Light

Stop

Speedlimit

Crosswalk.


## Prerequisites

- Python 3.7+
- Jupyter Notebook
- Required Python packages (see requirements.txt)

## Installation

1. Clone this repository:
```bash
git clone <repository-url>
cd road-sign-detection
```


## Usage

1. Install dependencies:
```bash
pip install -r requirements.txt
```

## Run the main notebook:
``` bash
jupyter notebook road-sign-detection.ipynb
```
## Features
Dataset exploration and visualization

XML annotation parsing

Sample image display

Road sign detection model implementation


## requirements.txt 
```bash
numpy>=1.21.0

pandas>=1.3.0

matplotlib>=3.5.0

opencv-python>=4.5.0

Pillow>=8.3.0

jupyter>=1.0.0
```
## Step-by-Step Execution
### Dataset Exploration: The notebook automatically explores the dataset structure and displays:

File organization

Sample images

XML annotation parsing

Dataset statistics

Data Analysis: The code includes functions to:

Load and display sample images

Parse PASCAL VOC XML annotations

Examine image dimensions and object counts

Visualize bounding boxes on images

Next Steps: The notebook outlines potential next steps for:

Processing annotations into training labels

Data splitting into train/validation/test sets

Data augmentation implementation

Model training for road sign detection

## Running Individual Components
### You can also run individual components from the source code:
``` bash
# Import and use data preprocessing functions
from src.data_preprocessing import parse_annotations, load_images

# Use utility functions
from src.utils import display_sample_images
```
# NOTE
The original IPython notebook with the complete dataset exploration code is provided as **road-sign-detection.ipynb**. This file contains the main analysis and should be used as the starting point for understanding the dataset and project workflow.


