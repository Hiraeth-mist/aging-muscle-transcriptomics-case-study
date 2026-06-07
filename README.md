# Transcriptomic Signatures of Skeletal Muscle Aging Across Distinct Muscle Types in Mice

## Project Overview

This project presents a complete bulk RNA-seq case study investigating age-associated transcriptional changes across multiple skeletal muscle types in mice. The analysis focuses on identifying differentially expressed genes, biological pathways, and shared molecular signatures of aging in fast-twitch, slow-twitch, and mixed muscle tissues.

The project was designed as a consulting-style bioinformatics case study, demonstrating an end-to-end workflow from data acquisition and quality assessment to biological interpretation and scientific communication.

---

## Biological Question

How does aging alter gene expression across different skeletal muscle types?

Specifically:

* Which genes are differentially expressed between young and aged muscle?
* Which biological pathways are disrupted during aging?
* Are aging signatures shared across muscle types or tissue-specific?
* What molecular mechanisms may contribute to age-related muscle decline?

---

## Dataset

**GEO Accession:** GSE287832

**Organism:** Mus musculus

**Technology:** Bulk RNA Sequencing (Illumina NovaSeq 6000)

**Muscle Types:**

* Extensor Digitorum Longus (EDL)
* Soleus
* Tibialis Anterior (TA)

**Experimental Design:**

* Young mice (n = 3)
* Aged mice (n = 3)

For each muscle type:

* 3 Young samples
* 3 Aged samples

Total samples analyzed: 18

---

## Analysis Workflow

1. Data acquisition from GEO
2. Import of Salmon quantification files
3. Construction of count matrices
4. Quality assessment and PCA
5. Differential expression analysis using DESeq2
6. Volcano plot generation
7. Heatmap visualization
8. Functional enrichment analysis
9. Cross-muscle comparison of aging signatures
10. Biological interpretation and reporting

---

## Tools and Packages

### R

* DESeq2
* tximport
* EnhancedVolcano
* pheatmap
* clusterProfiler
* enrichplot
* ggplot2

### Data Source

* GEO Omnibus (GSE287832)

---

## Planned Deliverables

### Bioinformatics Deliverables

* Differential expression analysis
* Principal component analysis (PCA)
* Volcano plots
* Heatmaps
* Gene Ontology enrichment
* Cross-muscle comparison analyses

### Communication Deliverables

* Scientific report
* Conference-style poster
* Research presentation
* GitHub case study

---

## Repository Structure

* notebooks/ : analysis notebooks
* scripts/ : reusable analysis scripts
* results/ : generated outputs
* figures/ : publication-quality figures
* report/ : consulting-style report
* poster/ : conference poster
* presentation/ : presentation slides

---

## Author

Akshat Jaiswal

M.Tech Biomedical Engineering, IIT Ropar

Interested in computational biology, transcriptomics, aging, regeneration, and bioinformatics.
