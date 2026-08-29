# Adversarial Attacks and Defenses

A practical study of **adversarial attacks and defense methods** for image classification using **PyTorch**, **CIFAR-10**, and **ResNet20**.

## Overview

This project investigates the vulnerability of deep neural networks to adversarial examples and evaluates several techniques for improving adversarial robustness.

The main experiments include:

### Adversarial Attacks

Four white-box attacks are implemented and evaluated:

* **FGSM** — Fast Gradient Sign Method
* **PGD** — Projected Gradient Descent
* **DeepFool**
* **C&W** — Carlini & Wagner \(L_2\) Attack

The main notebook implements these attacks directly with PyTorch.

### Defense Methods

Three defense approaches are evaluated:

* **Adversarial Training**
* **Randomized Smoothing**
* **Diffusion Purification**

The experiments compare both **clean accuracy** and **robust accuracy** under different attacks.

## Repository Structure

```text
.
├── 01-adversarial_attacks_and_defenses.ipynb
├── 02-adversarial_attacks_with_torchattack.ipynb
├── 03-adversarial_training_against_C&W_attack.ipynb
├── docs/
└── report.pdf
```

### Notebooks

**01 — Adversarial Attacks and Defenses**

Main experiment using CIFAR-10 and ResNet20. It includes implementations of FGSM, PGD, DeepFool, and C&W attacks, as well as adversarial training, randomized smoothing, and diffusion purification defenses.

**02 — Attacks with Torchattacks**

Uses the `torchattacks` library to evaluate **FGSM** and **PGD**, including comparisons between the clean model and an adversarially trained model.

**03 — Adversarial Training against C&W**

Experiments with adversarial training specifically against the **Carlini & Wagner attack**.

## Main Tools

* Python
* PyTorch
* Torchvision
* Torchattacks
* Diffusers
* NumPy
* Matplotlib
* Jupyter Notebook

## Running the Project

Clone the repository:

```bash
git clone https://github.com/alifathi11/adversarial-attacks-and-defenses.git
cd adversarial-attacks-and-defenses
```

Then start Jupyter:

```bash
jupyter notebook
```

and run the notebooks in the repository.

## Goal

The goal of this project is to experimentally study how adversarial perturbations affect image classifiers and compare different approaches for improving robustness against adversarial attacks.

