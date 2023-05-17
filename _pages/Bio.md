---
layout: page
title: About
permalink: /Bio/
---

Tipperary native first and foremost with an interest in computational biology. 

I have recently submitted my PhD thesis where I worked in Prof. Cathal Seoighes research group at the University of Galway. My PhD project aimed to infer the underlying effects of somatic mutations in relatively healthy populations such as the UK Biobank. To answer my research question, I built pipelines to download and analyse 200,000 whole exome sequenced samples (over 175Tb of raw input data!). 

I completed my undergraduated in biotechnology (2016) and MSc in Biomedical Genomics (2017) both in Galway. I spent 3 months of my third year of undergrad in Vannes, Brittany characterising the biochemical makeup of the burdensome *Solieria Chordalis* which washes ashore on the beaches of the northwest of France every year. For my undergraduate final year project I worked on trying to find variants associated with memory formation and schizophrenia under the supervision of Derek Morris. Coming from a "wet lab" undergraduate degree my final year project thought me that biological research was not solely pipetmans and tedious protocols but rather computers and statistics could create insights quite easily (and often from a coffee shop!). My masters thesis involved using simplistic methods to try and infer somatic mutation rates from population sequencing data and the germline variants that impact on the inferred somatic mutation rate. Throughout my MSc, I built a strong knowledge of cancer biology and statistics while developing a strong computational skillset. 

After graduating from my MSc (2018) I worked as a Bioinformatician at EMBL-EBI for the AMP-T2D project. My work on the AMP-T2D project mainly consisted of writing a Type II Diabetes GWAS pipeline to mirror the pipelines at the Broad Institute and push the association statistics to the federated knowledge base at EMBL-EBI. The federated node at the EBI allowed for European genetic data to be housed within Europe and summary level data to be shared to the knowledge portal hosted at the Broad institute ([AMPT2DKP](https://t2d.hugeamp.org/){:target="_blank"}) adhering to consent and European data policies. 

I returned to Galway to undertake a Irish research council funded PhD scholarship working somatic mutations from population sequencing projects. In 2020 I moved from the IRC post to an Science Foundation Ireland PhD scholarship within the same research group. During My PhD I have been acting as a defacto System administrator for two high performance compute clusters and all the fun that goes along with HPC administration. In 2019, I was awarded a  €25,000 small research equipment grant to contribute to a new high perfomance filesystem (250TB usuable storage). In the first year of my PhD I was a TA for probablistic modelling for molecular biology. This course covered topics such as Markov chain Monte Carlo methods and models of DNA evolution (Jukes & Cantor, Kimura's 2 parameter model,General time reversible etc...). 


**PhD Abstract**

*Somatic mutations accumulate throughout life and contribute significantly to disease
risk. While research into somatic mutation is well established in cancer, it is only in
recent years that investigations into the implications of somatic mutations in healthy
tissues have begun to be feasible, due to advances in sequencing technologies and pro-
tocols. The requirement of specialist techniques has, however, limited the study of
somatic mutations in healthy tissues to small sample sizes, which do not allow for as-
sessment of the impact of somatic mutations on human health on a population scale. We
posited that it may be possible to study variation in the somatic mutation rate between
individuals and across the genome through analysis of low-depth sequencing data, by
developing strategies to distinguish the contribution of somatic mutations to the mis-
matches (relative to the reference genome) observed in these data from sequencing
errors, DNA damage and other artefacts.

Using somatic mutation rates obtained from the literature, we estimated that 0.4%
of the mismatches between the UK Biobank exome sequencing reads and the refer-
ence genome were due to somatic mutations. We demonstrated that this proportion
was sufficient to induce a relationship between the abundance of mismatches and age,
when individuals were grouped by integer age. We then searched for additional sample
properties that are correlated with the mismatch burden and found positive correlations
with cancer diagnosis and smoking status. However, by carefully examining the UK
Biobank exome sequencing data, we uncovered previously unreported batch effects re-
lating to sequencing run. The observed associations with cancer diagnosis and smoking
status were lost when we corrected for this batch effect. However, the batch correction
improved the correlation between age and mismatch load.

Individuals diagnosed with Lynch syndrome have increased somatic mutation loads
due to deficiencies in mismatch repair genes and we investigated whether this effect
could be detected in the exome sequencing data. In the UK Biobank, we identified
160 individuals with pathogenic variants associated with Lynch syndrome. Using the
COSMIC signatures associated with mismatch repair, we compared the contribution
of mismatch repair mutational signatures between the Lynch syndrome samples and
the remaining samples. We detected a marginally statistically significant difference
between the contribution of SBS18 between the two sample groups; however, this result
did not survive multiple correction testing.*
