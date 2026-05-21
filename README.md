# Deep Learning for Michelson Interferometer Inverse Problems

Physics-informed deep learning models for forward and inverse problems in optical interferometry.

This project was developed as a final project for Brown University CS1470 (Deep Learning). The goal is to explore whether convolutional neural networks (CNNs) can learn the relationship between interference patterns and optical wavelengths in a Michelson interferometer system.

The repository investigates both:

- forward problems:
  - wavelength → interference pattern
- inverse problems:
  - interference pattern → wavelength

---

# Overview

A Michelson interferometer generates interference fringes whose spatial patterns depend on the optical wavelength and path-length difference.

Traditionally, wavelength extraction requires analytical signal processing or spectral analysis. In this project, deep neural networks are trained to directly infer wavelength information from raw interference images.

The framework combines:

- optical physics simulation
- synthetic data generation
- convolutional neural networks
- inverse regression
- image-based scientific machine learning

---

# Repository Structure

```text
data/
```

Training and testing datasets for interferometer images.

```text
generator/
```

Physics-inspired image generation scripts for interference patterns.

```text
models/
```

CNN architectures for forward and inverse prediction tasks.

```text
training/
```

Training scripts and optimization workflows.

```text
evaluation/
```

Prediction and visualization utilities.

---

# Physics Background

The Michelson interferometer produces interference fringes governed by optical path differences.

The intensity field can be approximated as:

$$
I \propto \cos^2\left(\frac{2\pi \Delta L}{\lambda}\right)
$$

where:

- $I$ is the optical intensity
- $\Delta L$ is the path-length difference
- $\lambda$ is the wavelength

The inverse problem attempts to recover $\lambda$ from the interference image.

---

# Machine Learning Tasks

## 1. Forward Problem

Predict or generate interference patterns from wavelength inputs.

```text
wavelength → interference image
```

This task explores learned optical pattern generation.

---

## 2. Inverse Problem

Predict wavelength values directly from interference images.

```text
interference image → wavelength
```

This is an image-based inverse regression problem.

---

# Features

- CNN-based inverse modeling
- Synthetic interferometer data generation
- Physics-inspired image simulation
- TensorFlow implementation
- Image regression workflow
- Scientific machine learning pipeline

---

# Deep Learning Framework

The project is implemented using:

- TensorFlow 2.2
- NumPy
- Matplotlib

The CNN models are trained on synthetic interferometer datasets generated from optical equations.

---

# Example Workflow

## Data Generation

Generate synthetic interference patterns for different wavelengths.

## Training

Train CNN models to predict wavelength values from images.

## Evaluation

Compare predicted wavelengths against ground-truth values.

---

# Educational Purpose

This project explores the intersection of:

- optics
- inverse problems
- scientific machine learning
- computer vision
- physics-informed AI

The implementation prioritizes conceptual understanding and experimentation.

---

# Possible Extensions

Potential future improvements include:

- physics-informed neural networks (PINNs)
- uncertainty quantification
- transformer-based vision models
- diffusion-based inverse reconstruction
- experimental interferometer calibration
- noise robustness analysis
- multi-wavelength reconstruction
- Fourier optics integration

---

# Related Topics

- Scientific Machine Learning
- Computational Imaging
- Optical Interferometry
- Inverse Problems
- Computer Vision
- Physics-Informed AI
- Deep Learning for Physics

---

# Requirements

Typical dependencies include:

```text
TensorFlow 2.2
NumPy
Matplotlib
OpenCV
```

---

# Author

Siyuan Song  
Brown University  
CS1470 Final Project  
Scientific Computing / Scientific ML
