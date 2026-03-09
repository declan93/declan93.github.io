---
layout: post
title: "ALTitude: a tabular foundation model for ALT classification nominates SMARCAL1 as a therapeutic target"
categories: [papers]
paper_ref: "Bennett D*, Wierdl M* et al. Tabular foundation-based model predicts alternative lengthening of telomeres (ALT) and identifies SMARCAL1 as a target in ALT-driven cancers. 2026."
excerpt: "A machine learning classifier trained on WGS-derived telomere features precisely identifies ALT-positive cancer cell lines at scale, enabling the first systematic CRISPR dependency analysis stratified by ALT status — and pointing to SMARCAL1 as a biomarker-matched target in paediatric solid tumours."
---

**Reference:** Bennett D\*, Wierdl M\* et al. Tabular foundation-based model predicts alternative lengthening of telomeres (ALT) and identifies SMARCAL1 as a target in ALT-driven cancers. *Preprint, 2026.*

---

## The Problem

Alternative Lengthening of Telomeres (ALT) is a recombination-based telomere maintenance mechanism active in roughly 10–15% of cancers, and substantially enriched in some of the most treatment-refractory paediatric tumours — osteosarcoma, rhabdomyosarcoma, high-risk neuroblastoma. No new systemic therapies have entered the clinic for osteosarcoma in over 40 years.

A major bottleneck in ALT target discovery has been classification itself. Standard ALT assays (C-circle, APBs, telomere FISH) are low-throughput, lab-intensive, and inapplicable at scale to the thousands of cell lines profiled in resources like the Cancer Dependency Map (DepMap). Without accurate, large-scale ALT annotations, CRISPR screen data cannot be stratified by ALT status — meaning potential biomarker-matched dependencies remain hidden in the noise.

---

## ALTitude: WGS-to-ALT at scale

Here we developed **ALTitude**, a classifier that infers ALT status in preclinical models from WGS alone, without paired germline sequencing, and with explicit correction for sequencing batch effects via PCA normalisation of the feature space.

Five feature categories are extracted from tumour WGS:

- TERT expression (low in ALT)
- Telomere length estimates
- Frequencies of 49 telomeric variant repeats (all 6-mer permutations of the TTAGGG unit)
- Telomere fusion rates
- Neo-telomere structure prevalence

Nine ML algorithms were benchmarked on 82 orthogonally validated cell lines (20 ALT+, 62 non-ALT) using leave-one-out cross-validation. **TabPFN2** — a tabular neural network foundation model — ranked first across ablation configurations (mean AUROC 0.965) and achieved AUROC 1.0 on a held-out test set with 100% precision and 100% sensitivity.

When applied to 935 DepMap cell lines with available WGS, ALTitude predicted 19 additional ALT+ models not in prior classifications, bringing the annotated total to 39 (4.2%), with the expected enrichment in undifferentiated pleomorphic sarcoma (67%) and osteosarcoma (53%). These labels are now publicly integrated into the DepMap portal.

---

## SMARCAL1: top CRISPR dependency in ALT+ cancers

With ALT labels in hand, the authors performed differential CRISPR dependency analysis across ~20,000 genes, comparing the 39 ALT+ lines against 896 non-ALT lines in DepMap genome-scale LOF screens.

**SMARCAL1 was the top hit** (FDR = 1.21 × 10⁻³⁰, β = −0.54). Among lines with moderate-to-strong SMARCAL1 dependency (CHRONOS < −0.35), 58% were ALT+. The dependency was most pronounced in rhabdomyosarcoma, osteosarcoma, and paediatric AML lineages.

Validation was extensive:
- CRISPR KO in ALT+ osteosarcoma and rhabdomyosarcoma lines reduced viability; ALT-negative lines were unaffected
- Two patient-derived ALT+ neuroblastoma models confirmed as dependent
- An acute dTAG degron system (FKBP12F36V-SMARCAL1) validated on-target effects
- A pooled in vivo CRISPR screen in Cal72 osteosarcoma xenografts scored SMARCAL1 as a significant hit (P = 0.05), with in vitro/in vivo screen correlation of Pearson r = 0.60

---

## ATRX and SMARCAL1 are functionally redundant SNF2 remodelers

A critical insight emerged from re-annotating ATRX/DAXX loss across DepMap. Simple variant calls severely overcall functional ATRX inactivation — only 24 of 138 lines with candidate variants showed likely complete canonical LOF after careful allele dosage, expression, and functional data integration. Of these, 20/24 (83%) were ALT+, and 16 were previously unreported disease models.

SMARCAL1 dependency did not differ significantly between ATRX-LOF and ATRX-intact ALT+ lines — it is a general ALT dependency. However, **ATRX/DAXX loss was markedly enriched** among SMARCAL1-dependent lines (35% vs. 0.7%, Fisher's P < 10⁻⁴). In ATRX-intact ALT+ cells, ATRX itself was the strong dependency — suggesting reciprocal functional compensation between the two proteins.

Rescue experiments confirmed this directly:
- SMARCAL1 overexpression in NY osteosarcoma (SMARCAL1-null, ATRX-WT) rescued the fitness cost of ATRX KO
- ATRX re-expression in OS384 osteosarcoma (ATRX-null) rescued SMARCAL1 dependency

Both proteins are SNF2-family ATP-dependent chromatin remodelers with conserved helicase domains and shared function at stalled replication forks — a mechanistically grounded basis for their redundancy at ALT telomeres.

---

## Mechanism: SMARCAL1 loss destabilises ALT beyond a tolerable threshold

RNA-seq after SMARCAL1 KO revealed a strikingly context-specific transcriptional response. In ALT+ G292 cells, SMARCAL1 loss amplified the ALT gene expression programme (NES +2.28, P = 1.3 × 10⁻⁷). In non-ALT Huh7 cells, there was no such effect. Non-ALT cells successfully engaged canonical DNA damage response and stress-response pathways; ALT+ cells could not.

Supporting data:
- C-circle accumulation increased post-SMARCAL1 depletion only in ALT+, SMARCAL1-dependent lines
- CHK1 phosphorylation (G2/M checkpoint) increased selectively in ALT+ lines, indicating checkpoint engagement the cells cannot resolve
- Flow cytometry showed S-phase and G2/M accumulation in ALT+ cells after CRISPRi
- Spectral karyotyping of OS384 post-CRISPRi showed significantly elevated chromosome counts — aneuploidy from mitotic catastrophe

The model: SMARCAL1 maintains ALT at a sustainable level; its loss pushes ALT beyond a threshold that ALT+ cells cannot tolerate, driving a cell death pathway that non-ALT cells are not exposed to.

---

## Why this matters

The paper delivers two interconnected resources. First, a practical, high-precision ALT classifier — publicly available, integrated into DepMap — that enables the field to stratify any WGS-profiled dataset by ALT status without orthogonal wet-lab assays. Second, a mechanistically grounded, preclinically validated target (SMARCAL1) for cancers where there has been essentially no therapeutic progress.

SMARCAL1 is encoded by a SNF2 ATPase. It is dispensable for normal development in mice, suggesting a potential therapeutic window. Related SNF2 ATPases are increasingly being pursued as drug targets, and the clear biomarker — ALT status, now detectable from WGS — provides a stratification strategy ready for translational application.

For ALT biology, the ATRX–SMARCAL1 functional redundancy story is a satisfying mechanistic closure: two SNF2 remodelers manage replication fork stress at ALT telomeres, loss of one shifts dependency onto the other, and both become vulnerabilities in a context-dependent manner.

---

## Looking ahead: from cell lines to patients

The cell line framework established here is now being extended to primary patient tumours. ALTitude was designed with this in mind — operating on somatic WGS without matched germline, and correcting for batch effects that are inevitable when aggregating data across clinical sequencing programmes. Applying the classifier to large paediatric cohorts (e.g., Pediatric Cancer Genome Project, TARGET, St. Jude Cloud) will establish the true prevalence of ALT across histologies at diagnosis and relapse, test whether ALT status associates with outcome independently of known risk factors, and — critically — identify the patient populations most likely to benefit from SMARCAL1-targeted therapy as it moves towards clinical development.
