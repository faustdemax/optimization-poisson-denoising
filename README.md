# Iterative Shrinkage for Poisson Noise Removal

This project implements and compares the **Poisson Iterative Shrinkage (PIS)** algorithm and the **Richardson-Lucy (RL)** algorithm for restoring images degraded by Poisson noise and blur.

## 📘 Reference
Shaked & Michailovich, *Iterative Shrinkage Approach to Restoration of Optical Imagery*, IEEE TIP 2011.

## 📂 Contents

- `Notebook de MAXIMY.ipynb` – Implementation and evaluation (metrics: NMSE, SSIM)
- `Data/` – Astronomical image and Shepp-Logan Phantom
- `Report DE MAXIMY.pdf` – Full technical report
- `paper.pdf` – Original research paper

## 🚀 Results

| Method         | NMSE    | SSIM   |
|----------------|---------|--------|
| Noisy image    | 0.1897  | 0.2316 |
| RL algorithm   | 0.1545  | 0.4417 |
| PIS algorithm  | 0.1853  | 0.2373 |

## 📌 Notes

- The code for optimal μ failed to converge; better results may be obtained with further tuning.
- This repo replicates the comparison on astronomical images and Phantom images.
