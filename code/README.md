# Computational Interferometry — Code

Deep learning models for forward and inverse problems in Michelson interferometry.

This project explores whether CNNs can learn the relationship between:

```text
wavelength ↔ interference pattern
```

using simulated interferometer images.

---

# Physics Background

The interference intensity approximately follows:

$$
I \propto \cos^2\left(\frac{2\pi \Delta L}{\lambda}\right)
$$

where $\lambda$ is the optical wavelength.

The inverse problem attempts to recover wavelength information directly from interference images.

---

# Structure

```text
data_generation.py   # generate synthetic interferometer images
train.py             # train CNN model
evaluate.py          # evaluate prediction performance
models/              # saved models
data/                # generated datasets
```

---

# Installation

```bash
git clone https://github.com/ssong26/Computational_Interferometry.git
cd Computational_Interferometry/code

pip install tensorflow numpy matplotlib opencv-python
```

Recommended environment:

```text
Python 3.7+
TensorFlow 2.2
```

---

# Usage

## Generate Dataset

```bash
python data_generation.py
```

## Train Model

```bash
python train.py
```

## Evaluate Model

```bash
python evaluate.py
```

---

# Topics

- Computational Imaging
- Optical Interferometry
- Inverse Problems
- Scientific Machine Learning
- Physics-Informed AI

---

# Author

Siyuan Song  
Brown University
