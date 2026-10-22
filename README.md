# Rare Disease Hackathon 2026 - Track 1 Solution
**Team Name:** profetas  
**Target Disease:** Mosaic Variegated Aneuploidy (MVA) / CEP57 & BUB1B  

## Overview
This repository contains the full end-to-end genomic variant filtering, prioritization, and machine learning pipeline for Track 1 of the SageBio MVA Hackathon 2026.

## Structure
- `1_descarga_datos.ipynb`: Dataset download script from Hugging Face Hub.
- `2_filtrado_variantes.ipynb`: Local VCF processing, PASS quality filtering, and isolation of 357 truncating (Loss-of-Function) variants.
- `3_priorizacion_ml.ipynb`: Machine learning classification and ACMG/CADD prioritization framework.
- `4_validacion_y_reporte.ipynb`: Feature importance, chromosome distribution analysis, and clinical report generation.
- `profetas_track1_submission.csv`: Final semicolon-delimited prediction file for Hugging Face submission.
- `profetas_methods_description_form.xlsx`: Official methods description form.

## How to Run
1. Install dependencies:
   ```bash
   pip install huggingface_hub notebook ipykernel pandas numpy scikit-learn scikit-allel pysam openpyxl