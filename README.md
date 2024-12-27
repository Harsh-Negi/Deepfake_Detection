# Deepfake Detection Project

This repository contains the code for a Convolutional Neural Network (CNN) model designed to classify images as 'Real' or 'Fake' (Deepfakes). The project leverages a dataset of manipulated and real face images, achieving high accuracy through effective preprocessing and training techniques.

## Features

- Image classification using a CNN architecture.
- Preprocessing techniques: resizing, grayscale conversion, and normalization.
- Batch processing for efficient training.
- Utilizes categorical cross-entropy loss for classification tasks.

## Dataset

The dataset used in this project consists of:

- **190,000 images** (manipulated and real faces).
- Resolution: 256x256 pixels.

### Dataset Access
The dataset is available on Kaggle:
[Deepfake and Real Images Dataset](https://www.kaggle.com/datasets/manjilkarki/deepfake-and-real-images).

### Dataset Preparation
After downloading the dataset:

1. Ensure all images are in the `256x256` resolution.
2. Convert images to grayscale.
3. Normalize the pixel values to the range `[0, 1]`.

You can use the provided preprocessing scripts in the `scripts/` folder for these steps.

## Getting Started

### Prerequisites

- Python 3.x
- TensorFlow/Keras
- NumPy
- Matplotlib
- OpenCV (for image preprocessing)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/deepfake-detection.git
   cd deepfake-detection
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Prepare the dataset and place it in the `data/` directory (not included in the repository).
2. Run the training script:
   ```bash
   python train.py
   ```
3. Evaluate the model:
   ```bash
   python evaluate.py
   ```

### Results

- Training accuracy: **[Insert value]**
- Validation accuracy: **[Insert value]**
- Sample visualizations of predictions are available in the `results/` directory.

## Directory Structure

```
.
├── data/               # Directory for dataset (not included)
├── models/             # Saved models
├── scripts/            # Preprocessing scripts
├── results/            # Visualizations and logs
├── train.py            # Script for training the model
├── evaluate.py         # Script for evaluating the model
├── requirements.txt    # Dependencies
└── README.md           # Project documentation
```

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/manjilkarki/deepfake-and-real-images).
- Special thanks to the creators and contributors of the dataset.
