# Deep Learning Project 3: Adversarial Attacks on ResNet-34

This repository contains the implementation of various adversarial attacks against a pre-trained ResNet-34 model as part of the Deep Learning Project 3 (Spring 2025).

## Project Overview

The goal of this project is to implement effective adversarial attacks that degrade the performance of a pre-trained ResNet-34 model while ensuring the perturbations remain imperceptible. We focus on:

1. **Basic Model Evaluation**: Testing ResNet-34 on ImageNet classes 401-500
2. **FGSM Attack**: Fast Gradient Sign Method with ε = 0.02
3. **Enhanced PGD Attack**: Modified Projected Gradient Descent targeting top-5 evasion
4. **Patch Attack**: Concentrated attacks on small image regions (to be implemented)
5. **Transferability Analysis**: Testing attacks across different model architectures (to be implemented)

## Repository Structure

- `notebooks/`: Jupyter notebooks implementing the tasks
- `results/`: Performance metrics and visualizations

## Tasks and Results

### Task 1: Model Evaluation
Evaluation of ResNet-34 on our custom test dataset to establish baseline performance.

### Task 2: FGSM Attack
Implementation of the Fast Gradient Sign Method (FGSM) attack with ε = 0.02, creating imperceptible adversarial perturbations.

### Task 3: Enhanced PGD Attack
An improved attack using Projected Gradient Descent with momentum specifically designed to remove the true class from the top-5 predictions.

### Task 4: Patch Attack
Concentrated attacks on small 32x32 regions of the image.

### Task 5: Transferability Analysis
Evaluation of how our adversarial examples transfer to other model architectures.

## Key Results

| Dataset | Top-1 Accuracy | Top-5 Accuracy |
|---------|---------------|---------------|
| Original Test Set | TBD | TBD |
| Adversarial Test Set 1 (FGSM) | TBD | TBD |
| Adversarial Test Set 2 (Enhanced PGD) | TBD | TBD |
| Adversarial Test Set 3 (Patch Attack) | TBD | TBD |

## Requirements

The code was tested with the following requirements:
```
torch>=2.0.0
torchvision>=0.15.0
numpy>=1.23.0
matplotlib>=3.5.0
pillow>=9.0.0
tqdm>=4.64.0
```

To install the dependencies:
```
pip install -r requirements.txt
```

## Usage

Each notebook is self-contained and can be run independently:

1. First install the requirements.
2. Then run `notebooks/dl-project-3-adversarial-attacks.ipynb` to establish all five tasks.


## Team Members
- Karthik Krapa ()
- Krish Murjani (km6520)
- Pratham Saraf (ps5218)

