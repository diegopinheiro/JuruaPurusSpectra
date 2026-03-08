# JuruaPurusSpectra

Hyperspectral analysis of PRISMA imagery and laboratory spectroscopy for soil and water characterization in riverbank environments of the Juruá and Purus rivers, Brazilian Amazon.

## Overview

This repository contains data, scripts, and methodological notes related to the evaluation of **PRISMA hyperspectral imagery** for the characterization of:

- exposed riverbank soils and sediments
- water optical conditions
- spectral correspondence between orbital and laboratory measurements

The study is based on field campaigns conducted in:

- **Boca do Acre** (Purus River)
- **Itamarati** (Juruá River)
- **Ipixuna** (Juruá River)

## Objective

The main objective of this repository is to support the comparison between:

1. **PRISMA surface reflectance imagery**
2. **ASD FieldSpec laboratory spectra** collected from soil samples
3. **Secchi depth measurements** used as an indicator of water transparency

## Study context

Amazon floodplains are challenging environments for optical remote sensing because of:

- turbid waters
- exposed sediments
- cloud and haze interference
- mixed pixels
- strong spatial heterogeneity along riverbanks

This repository was created to organize a site-specific spectral reference dataset for riverbank environments in the western Brazilian Amazon.

## Data sources

### Field data
- georeferenced soil sampling points
- Secchi depth measurements collected in situ
- observations from sandy and clayey riverbank surfaces

### Laboratory data
- oven-dried soil samples
- ASD FieldSpec spectral measurements
- spectral range from 350 to 2500 nm
- repeated scans with calibration using a Lambertian reference panel

### Orbital data
- PRISMA Level-2D imagery
- spectral extraction using EnMAP-Box and QGIS
- point-based comparison with georeferenced sample locations

## Methods

The workflow includes:

- PRISMA image processing
- extraction of spectral profiles from sample points
- harmonization between FieldSpec and PRISMA spectral bands
- exclusion of problematic absorption ranges
- spectral similarity analysis using:
  - SAM
  - RMSE
  - Pearson correlation
- exploratory analysis of PRISMA water reflectance against Secchi depth

## Repository structure

```text
JuruaPurusSpectra/
├── data/
├── scripts/
├── figures/
├── outputs/
└── README.md
