# Comparative Transcriptomic Analysis of Skeletal Muscle Aging in Mice

## Executive Summary

Aging is associated with progressive loss of skeletal muscle mass and function, a condition known as sarcopenia. Understanding the molecular mechanisms underlying muscle aging is critical for identifying potential therapeutic targets.

This study analyzed publicly available RNA-seq data from three mouse skeletal muscle types:

* Extensor Digitorum Longus (EDL)
* Soleus
* Tibialis Anterior (TA)

Differential expression and functional enrichment analyses were performed to characterize aging-associated transcriptional changes.

Key findings indicate that EDL undergoes extensive transcriptional remodeling during aging, whereas Soleus exhibits relative resistance and TA demonstrates an intermediate response.

---

## Introduction

### Background

Sarcopenia is a major contributor to age-associated frailty and loss of mobility. Although skeletal muscles share common physiological functions, individual muscle types differ in fiber composition, metabolic properties, and susceptibility to aging.

The objective of this study was to compare aging-associated transcriptomic changes across multiple skeletal muscle types.

---

## Dataset Description

### GEO Accession

GSE287832

### Organism

Mus musculus

### Experimental Design

18 RNA-seq samples

* Young mice
* Aged mice

Muscles analyzed:

* EDL
* Soleus
* TA

Three biological replicates per condition.

---

## Methods

### Quality Control

* Variance stabilizing transformation
* Principal Component Analysis
* Sample distance heatmap

### Differential Expression

DESeq2

Thresholds:

* Adjusted p-value < 0.05
* |log2 Fold Change| > 1

### Functional Enrichment

clusterProfiler

Gene Ontology Biological Process enrichment analysis.

---

## Results

### Quality Assessment

PCA demonstrated clear separation among muscle types and age groups.

Sample distance heatmaps confirmed high within-group similarity and strong biological clustering.

### Differential Expression

EDL:

* 1129 significant genes

Soleus:

* 44 significant genes

TA:

* 105 significant genes

EDL displayed the strongest transcriptional response to aging.

### Biomarker Discovery

Top differentially expressed genes successfully separated young and aged samples within each muscle type.

Heatmap analyses revealed distinct aging-associated expression signatures.

### Functional Enrichment

EDL:

* Muscle development
* TGF-beta signaling
* Growth regulation
* Apoptotic signaling
* Cytoskeletal remodeling

Soleus:

* Extracellular matrix organization
* Angiogenesis
* Vascular development

TA:

* Muscle differentiation
* Response to activity
* Response to muscle stretch

---

## Biological Interpretation

Distinct skeletal muscle types exhibit markedly different responses to aging.

EDL appears highly susceptible to aging-associated remodeling.

Soleus demonstrates relative transcriptional resilience.

TA exhibits an intermediate phenotype while maintaining muscle-specific adaptive pathways.

These observations suggest that muscle fiber composition and physiological function influence aging susceptibility.

---

## Conclusions

1. Skeletal muscle aging is strongly muscle-type specific.
2. EDL exhibits extensive transcriptomic remodeling during aging.
3. Soleus displays relative resistance to aging-associated transcriptional disruption.
4. TA maintains adaptive muscle-development pathways despite aging.
5. Functional enrichment analysis identifies distinct biological processes underlying aging in different muscle groups.

---

## Reproducibility

Analysis was performed using:

* R
* DESeq2
* clusterProfiler
* enrichplot
* pheatmap
* ggplot2

All code and outputs are available in the accompanying GitHub repository.
