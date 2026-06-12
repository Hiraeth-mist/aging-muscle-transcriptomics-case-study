# Comparative Transcriptomic Analysis of Skeletal Muscle Aging in Mice

## Project Overview

This project investigates aging-associated transcriptomic changes across three skeletal muscle types in mice using RNA-seq data.

The goal was to identify:

* Differentially expressed genes associated with aging
* Muscle-specific aging signatures
* Biological pathways altered during aging
* Differences in aging susceptibility across muscle types

The analysis was performed using publicly available RNA-seq data from GEO (GSE287832).

---

## Biological Question

Sarcopenia, the age-associated decline in muscle mass and function, affects different skeletal muscles to varying degrees.

Can transcriptomic analysis reveal why some muscles appear more susceptible to aging than others?

---

## Dataset

**GEO Accession:** GSE287832

**Organism:** Mus musculus

### Muscles Analyzed

* EDL (Extensor Digitorum Longus)
* Soleus
* TA (Tibialis Anterior)

### Samples

18 RNA-seq samples

* Young mice
* Aged mice

3 biological replicates per muscle-age combination

---

## Analysis Workflow

### 1. Quality Control

* Variance Stabilizing Transformation (VST)
* Principal Component Analysis (PCA)
* Sample Distance Heatmap

### 2. Differential Expression Analysis

* DESeq2
* Adjusted p-value < 0.05
* |log2 Fold Change| > 1

### 3. Biomarker Discovery

* Volcano Plots
* Top Differentially Expressed Genes
* Expression Heatmaps

### 4. Functional Enrichment

* Gene Ontology (GO)
* clusterProfiler
* enrichplot
* GO Network Analysis

### 5. Cross-Muscle Comparison

* Differential expression comparison
* Pathway comparison
* Aging susceptibility assessment

---

## Key Results

### Differentially Expressed Genes

| Muscle | Significant Genes |
| ------ | ----------------- |
| EDL    | 1129              |
| Soleus | 44                |
| TA     | 105               |

EDL exhibited the strongest aging-associated transcriptional remodeling.

---

### Functional Enrichment

#### EDL

* Muscle organ development
* TGF-beta signaling
* Growth regulation
* Apoptotic signaling
* Cytoskeletal remodeling

#### Soleus

* Extracellular matrix organization
* Angiogenesis
* Vasculature development

#### TA

* Muscle differentiation
* Response to activity
* Response to muscle stretch

---

## Major Biological Findings

### EDL

EDL displayed extensive transcriptomic remodeling during aging, suggesting high susceptibility to age-associated degeneration.

### Soleus

Soleus exhibited comparatively limited transcriptional disruption and appeared relatively resistant to aging.

### TA

TA maintained strong muscle-specific adaptive pathways despite aging, representing an intermediate phenotype.

---

## Repository Structure

```text
notebooks/
├── 01_data_import_qc.ipynb
├── 02_differential_expression.ipynb
├── 03_volcano_plots.ipynb
├── 04_biomarker_heatmaps.ipynb
├── 05_functional_enrichment_analysis.ipynb
├── 06_cross_muscle_comparison.ipynb

results/
├── pca/
├── volcano/
├── heatmaps/
├── enrichment/
├── comparison/

report/
└── Aging_Muscle_Case_Study_Report.md
```

## Tools Used

* R
* DESeq2
* clusterProfiler
* enrichplot
* pheatmap
* ggplot2
* dplyr

---

## Reproducibility

All analyses were performed using reproducible workflows in Google Colab and R.

The complete code, figures, tables, and report are provided within this repository.
