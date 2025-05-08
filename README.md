# Deep Learning Project 3
## Jailbreaking Deep Models (Spring 2025)
__Authors: Gaurav Kuwar, Stephen Chen, Yanka Sikder__

This project implements adversarial attacks on a pretrained ResNet-34 classifier using a subset of the ImageNet-1K dataset.

## Tasks

1. **Evaluation**: Compute top-1 and top-5 accuracy on the clean dataset.
2. **FGSM Attack**: Apply Fast Gradient Sign Method with ε = 0.02 to create Adversarial Test Set 1.
3. **Improved Attacks**: Implement stronger attacks (iterative FGSM, targeted FGSM, iterative targeted FGSM, PGD) to degrade accuracy further (Adversarial Test Set 2).
4. **Patch Attacks**: Apply attacks to only a 32×32 patch (Adversarial Test Set 3).
5. **Transferability**: Evaluate all datasets on another model (DenseNet-121).

### Accuracy Comparison - Resnet32

| Dataset              | Top-1 Accuracy (%) | Top-5 Accuracy (%) |
|----------------------|--------------------|---------------------|
| Task 1: Baseline  | 76.00               | 94.00                |
| Task 2: FGSM                 | 6.80               | 35.60                |
| Task 3: Improved attacks      | 0.00               | 9.00                |
| Task 4: Patch attacks        | 4.00               | 34.80                |


### Accuracy Comparison - DenseNet121

| Dataset              | Top-1 Accuracy (%) | Top-5 Accuracy (%) |
|----------------------|--------------------|---------------------|
| Task 1: Baseline  | 75.40               | 93.60                |
| Task 2: FGSM                 | 63.60               | 88.80                |
| Task 3: Improved attacks      | 64.60               | 90.40                |
| Task 4: Patch attacks        | 61.80               | 85.60                |