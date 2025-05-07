# Deep Learning Project 3
## Jailbreaking Deep Models (Spring 2025)
__Authors: Gaurav Kuwar, Stephen Chen, Yanka Sikder__

This project implements adversarial attacks on a pretrained ResNet-34 classifier using a subset of the ImageNet-1K dataset.

## Tasks

1. **Evaluation**: Compute top-1 and top-5 accuracy on the clean dataset.
2. **FGSM Attack**: Apply Fast Gradient Sign Method with ε = 0.02 to create Adversarial Test Set 1.
3. **Improved Attacks**: Implement stronger attacks (e.g., iterative FGSM) to degrade accuracy further (Adversarial Test Set 2).
4. **Patch Attacks**: Apply attacks to only a 32×32 patch (Adversarial Test Set 3).
5. **Transferability**: Evaluate all datasets on another model (e.g., DenseNet-121).