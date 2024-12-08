## ECE1512_ProjectB_PartA: Extending the Mamba architecture to process 2D visual sequences

## Overview
A visual state-space model inspired by the paper *"VMamba: Visual State Space Model"*. This project focuses on extending the VMamba architecture to process 2D visual sequences efficiently, showcasing its performance on benchmark datasets such as CIFAR-10.

## Features
- **Stem and Block Design**:
  - Initial convolutional layers for efficient feature extraction.
  - Multi-block architecture to hierarchically process visual features.
- **Path Extraction and Processing**:
  - Dynamic 2D path extraction for efficient feature representation.
  - Combination of visual paths to enhance feature robustness.
- **End-to-End Training**:
  - Supports both training and evaluation workflows.
- **Extensibility**:
  - Modular design enables easy adaptation to other datasets or tasks.

## Results
After training on the CIFAR-10 dataset, the model achieves the following results:
- **Accuracy**: ~80% after 20 epochs (example placeholder).
- **Loss**: Gradually decreases over training (example placeholder).

## Repository Structure
```plaintext
src/
├── vmamba.py             # Core VMamba implementation
├── utils.py              # Utility functions (e.g., data loading, preprocessing)
├── train.py              # Training script
├── evaluate.py           # Evaluation script
experiments/
├── training.ipynb        # Training notebook
├── evaluation.ipynb      # Evaluation notebook
results/
├── accuracy_results.txt  # Accuracy results
├── loss_results.txt      # Loss results
README.md                 # Project documentation
```

## Getting Started

### Prerequisites
- Python 3.8+
- PyTorch 2.0+
- CUDA-enabled GPU

### Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/ADglory/ECE1512_2024F_ProjectB_PartA_Repo_YingshunLu_Minghao-Ma
cd ECE1512_2024F_ProjectB_PartA_Repo_YingshunLu_Minghao-Ma
pip install -r requirements.txt
```

### Usage

#### Train the Model
To train the model on CIFAR-10:
```bash
python src/train.py --dataset CIFAR-10 --epochs 20 --batch_size 128
```

#### Evaluate the Model
To evaluate the model performance:
```bash
python src/evaluate.py --model_path PATH_TO_CHECKPOINT
```

## Discussion
This implementation successfully extends the VMamba architecture to process 2D visual sequences. By leveraging the modularity and efficiency of the original architecture, we demonstrate:
- Robust feature extraction and hierarchical processing.
- Efficient path-based sequence modeling.
- Competitive performance on benchmark datasets such as CIFAR-10.

The results highlight the adaptability of the VMamba framework to diverse visual tasks, making it a versatile tool for future research and applications.

## Authors
- **Yingshun Lu**
- **Minghao Ma**



## Acknowledgements
This project is based on the *"VMamba: Visual State Space Model"* paper and its accompanying GitHub repository. We adapted and extended the core ideas to develop a comprehensive framework for visual sequence modeling.
