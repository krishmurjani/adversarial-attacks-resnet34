# Results Directory

This directory contains the evaluation results and visualizations from our adversarial attacks on the ResNet-34 model.

## Metrics Format

The JSON files in the `metrics/` directory contain structured performance metrics for each task, generally following this format:

```json
{
  "top1_accuracy": 85.2,          // Top-1 accuracy percentage
  "top5_accuracy": 97.6,          // Top-5 accuracy percentage
  "total_images": 500,            // Total number of images evaluated
  "attack_parameters": {          // Parameters used for the attack (if applicable)
    "epsilon": 0.02,              // Attack budget
    "steps": 10                   // Number of steps (for iterative attacks)
  }
}
```

For attack result files, additional metrics may include:
- Accuracy drop compared to baseline
- Attack success rate
- L∞ distance statistics

## Visualizations

The visualization files in the `visualizations/` directory show sample results from our attacks:

- Each row typically shows a triplet of images:
  1. **Original Image**: The unmodified test image with its true class
  2. **Adversarial Image**: The perturbed image with its (incorrect) model prediction
  3. **Perturbation**: Magnified difference between original and adversarial images

The perturbations are usually magnified by a factor of 10x to make them visible, as the actual modifications are imperceptible to the human eye.

## Usage

These results can be used to:
- Compare the effectiveness of different attack methods
- Analyze how perturbation size affects attack success
- Visualize the nature of adversarial perturbations
- Support the findings and claims in the project report
