# PPDbench: Benchmarking of Different Molecular Docking Methods for Protein–Peptide Docking

## Overview

PPDbench is a benchmarking framework developed for evaluating molecular docking methods used in protein–peptide interaction studies.

Protein–peptide interactions play important roles in:

- Cell signaling
- Immune response
- Apoptosis
- Structural regulation
- Peptide therapeutics
- Drug discovery

This study systematically benchmarked six widely used docking methods on experimentally validated protein–peptide complexes using CAPRI evaluation criteria.

---

# Research Paper Details

## Title
Benchmarking of Different Molecular Docking Methods for Protein–Peptide Docking

## Authors
- Piyush Agrawal
- Harinder Singh
- Hemant Kumar Srivastava
- Sandeep Singh
- Gaurav Kishore
- Gajendra P. S. Raghava

## Journal
BMC Bioinformatics

## Publication Year
2019

## DOI
https://doi.org/10.1186/s12859-018-2449-y
https://doi.org/10.5281/zenodo.20200924
---

# Abstract

Protein–peptide docking is challenging because peptides are highly flexible and can adopt multiple conformations. Existing benchmarking studies mostly focus on protein–protein or protein–ligand docking, while very limited work has been done specifically for protein–peptide docking.

This study benchmarked six docking methods on 133 non-redundant protein–peptide complexes and evaluated their performance using:

- FNAT
- I-RMSD
- L-RMSD

The study demonstrated that:

- FRODOCK performs best for blind docking
- ZDOCK performs best for re-docking
- Existing scoring functions still require major improvements

A web-based benchmarking server named **PPDbench** was also developed.

---

# Docking Methods Evaluated

| Docking Method | Type |
|---|---|
| ZDOCK 3.0.2 | FFT-based rigid docking |
| FRODOCK 2.0 | Rigid-body docking |
| Hex 8.0.0 | Spherical Fourier docking |
| PatchDock 1.0 | Geometry-based docking |
| ATTRACT | Flexible docking |
| pepATTRACT | Protein–peptide docking |

---

# Dataset Information

## PPDbench Dataset

The benchmark dataset contains:

- 133 non-redundant protein–peptide complexes
- Peptide length between 9–15 residues
- Less than 40% sequence similarity

Dataset sources:

- peptiDB
- ACCLUSTER dataset

Redundancy removal tool:

- CD-HIT

---

# Evaluation Parameters

The docking performance was evaluated using CAPRI criteria.

## FNAT
Fraction of native contacts preserved.

## I-RMSD
Interface Root Mean Square Deviation.

## L-RMSD
Ligand Root Mean Square Deviation.

---

# Blind Docking Results

Blind docking was performed without prior binding-site information.

## Best Performing Method

### FRODOCK

| Metric | Value |
|---|---|
| Average L-RMSD (Top Pose) | 12.46 Å |
| Average L-RMSD (Best Pose) | 3.72 Å |

---

# Re-Docking Results

Re-docking was performed using known binding-site information.

## Best Performing Method

### ZDOCK

| Metric | Value |
|---|---|
| Average L-RMSD (Top Pose) | 8.60 Å |
| Average L-RMSD (Best Pose) | 2.88 Å |

---

# Key Findings

- FRODOCK performs best for blind docking
- ZDOCK performs best for re-docking
- Scoring functions are still not reliable enough
- Many methods generate good poses but rank them poorly
- Combining multiple docking methods improves performance
- Flexible peptides are more difficult to dock
- Higher-resolution crystal structures improve benchmarking quality

---

# Secondary Structure Analysis

Peptides were divided into:

- Regular secondary structure peptides
- Coil-dominated peptides

## Observation

Most docking methods performed better on:

- Coil-dominated peptides

Possible reason:

- Higher conformational adaptability

---

# Rotatable Bond Analysis

The study evaluated the effect of peptide flexibility.

## Findings

- Docking accuracy decreases with increasing rotatable bonds
- FRODOCK and ZDOCK handled flexibility better than other methods

---

# Reproducibility Analysis

Docking experiments were repeated multiple times.

## Observation

- Most docking methods produced highly reproducible results
- Performance differences between repeated experiments were negligible

---

# Web Server

## PPDbench Server

The study developed a web-based benchmarking platform.

### Features

- Single complex evaluation
- Batch evaluation
- FNAT calculation
- I-RMSD calculation
- L-RMSD calculation
- Benchmark dataset download

## Web Link

http://webs.iiitd.edu.in/raghava/ppdbench/

---

# Applications

PPDbench can be used for:

- Protein–peptide interaction studies
- Benchmarking docking software
- Peptide therapeutic design
- Drug discovery
- Structural bioinformatics
- Computational biology research

---

# Technologies Used

- Molecular Docking
- CAPRI Evaluation Framework
- FFT Docking Algorithms
- Spherical Harmonics
- Structural Bioinformatics
- Flexible Docking
- CD-HIT Clustering

---

# Conclusion

PPDbench provides a comprehensive framework for benchmarking protein–peptide docking methods.

The study highlights:

- Strengths and weaknesses of current docking methods
- Need for improved scoring functions
- Importance of benchmarking datasets
- Challenges in docking pose ranking

The developed web server provides valuable resources for researchers working in structural bioinformatics and peptide therapeutics.

---

# Citation

Agrawal P, Singh H, Srivastava HK, Singh S, Kishore G, Raghava GPS.

Benchmarking of different molecular docking methods for protein-peptide docking.

BMC Bioinformatics. 2019;19(Suppl 13):426.

DOI: https://doi.org/10.1186/s12859-018-2449-y

---

# Contact

## Dr. G. P. S. Raghava

Email: raghava@iiitd.ac.in

Address:  
Indraprastha Institute of Information Technology Delhi

---

# License

This project/documentation is intended for academic and research purposes only.
