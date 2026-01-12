---
layout: page
title: Research
permalink: /Research/
---

My research focuses on applying computational and machine learning methods to identify therapeutic vulnerabilities in pediatric cancers. I work at St. Jude Children's Research Hospital, leveraging large-scale genomic data and CRISPR screening to accelerate precision medicine.

---

## Current Research

### Pediatric Dependency Map (PedDep)
**St. Jude Children's Research Hospital** | 2024–Present

I lead computational analysis for the Pediatric Dependency Map project, a pediatric extension to the Broad Institute's DepMap initiative. This project characterizes ~300 pediatric cancer cell lines using:

- **CRISPR knockout screens** to identify genetic dependencies
- **Whole genome sequencing** for comprehensive mutation profiling
- **RNA sequencing** including long-read technologies
- **Epigenomic profiling** to understand regulatory landscapes

Our goal is to accelerate precision medicine by identifying novel therapeutic targets and drug combinations specific to pediatric malignancies.

---

### ALTitude: Predicting Telomere Maintenance Mechanisms

Cancer cells must overcome the end-replication problem to achieve replicative immortality. While 85-90% of cancers activate telomerase (TERT), 10-15% use **Alternative Lengthening of Telomeres (ALT)**—a recombination-based mechanism associated with poor prognosis in neuroblastoma, osteosarcoma, and soft tissue sarcomas.

**ALTitude** is a machine learning framework I developed to predict ALT status from whole-genome sequencing data. Key findings include:

- **Accurate ALT prediction** across 1,600+ cancer cell lines using telomeric features
- **ATRX loss-of-function** is enriched in ALT+ tumors but ~30% of ATRX-mutant samples are ALT-negative
- **SMARCAL1 as a therapeutic vulnerability**: ALT+ cancers with ATRX loss show synthetic lethality with SMARCAL1 depletion
- **Lineage-specific effects** in SMARCAL1 dependency patterns

This work positions St. Jude to identify and validate therapeutic targets in ALT+ pediatric cancers, which are enriched in solid tumors like neuroblastoma and osteosarcoma.

---

### Extrachromosomal DNA (ecDNA) in Neuroblastoma

I'm investigating ecDNA and its role in pediatric cancers, particularly:

- **MYCN amplification** occurs in ~40% of high-risk neuroblastoma cases
- ecDNA enables rapid copy number changes and drug resistance
- Developing computational methods to detect and characterize ecDNA from WGS data

---

## Previous Research

### Somatic Mutations in Population Sequencing
**University of Galway** | PhD Research

My doctoral work investigated somatic mutational processes in healthy populations using UK Biobank exome data (200,000+ samples). Key contributions:

- Demonstrated that ~0.4% of sequencing mismatches are attributable to somatic mutations
- Discovered previously unreported batch effects in UK Biobank sequencing data
- Investigated Lynch syndrome signatures in population-scale data
- Developed methods to distinguish somatic mutations from sequencing artifacts

### GWAS Method Development
**University of Galway** | PhD Research

- Developed polygenic scoring methods that improve GWAS statistical power
- Demonstrated that controlling for background genetic effects increases discovery of trait-associated variants

### AMP-T2D Bioinformatics
**EMBL-EBI** | 2018

- Built GWAS pipelines for the Accelerating Medicines Partnership - Type 2 Diabetes project
- Developed federated data analysis infrastructure to enable European genetic data to remain within Europe while contributing summary statistics to the AMP-T2D Knowledge Portal

---

## Technical Expertise

<div class="skills-grid">

**Cancer Genomics**
- CRISPR screen analysis (knockout, CRISPRi)
- Somatic mutation calling & signature analysis
- Telomere biology & ALT detection
- ecDNA characterization

**Computational Methods**
- Machine learning (scikit-learn, XGBoost)
- Statistical modeling (R, Julia)
- Pipeline development (Snakemake, Nextflow)
- Large-scale data analysis

**Data Resources**
- Pediatric Dependency Map (PedDep)
- DepMap / Cancer Cell Line Encyclopedia
- UK Biobank, TCGA, GTEx, ICGC
- TARGET pediatric cancer data

**Infrastructure**
- HPC cluster administration
- Cloud computing (AWS, GCP)
- Containerization (Docker, Singularity)

</div>

---

## Collaborations

I work closely with experimental labs at St. Jude to validate computational predictions, including:

- **Geeleher Lab** - Drug response prediction and pharmacogenomics
- **Guenther Lab** - ALT biology and telomere maintenance
- Collaborative projects across the Department of Computational Biology
