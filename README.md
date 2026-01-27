# Transcriptomic Atlas of Retinal Pathology in 5xFAD Mice

### A Time-Resolved Analysis of Alzheimer's Disease Progression
**Author:** Taye Motunrayo Ilesanmi  
**Status:** Manuscript in Preparation  

---

## Overview
This repository contains the visual assets and data visualizations generated for the study: **"Biphasic Progression of Retinal Pathology in Alzheimer's Disease."**

By analyzing the retinal transcriptome of 5xFAD mice at two distinct timepoints—**1.5 months (Prodromal)** and **6 months (Established Pathology)**—this project reveals that retinal neurodegeneration is not a linear decline. Instead, it follows a **biphasic trajectory**: an early phase of active synaptic compensation followed by a terminal phase of metabolic collapse and reactive gliosis.


### 1. The "Fighting" Phase (1.5 Months)
Insight: The retina exhibits a robust homeostatic response (GO: Synaptic Organization) masking a hidden metabolic deficit.


![GO terms at 1.5M](figures/combined_ORAdotplots(1M).png)


However, Gene Set Enrichment Analysis (GSEA) reveals a "hidden" crisis: a subtle but coordinated downregulation of Oxidative Phosphorylation that standard methods missed.

![GSEA result at 1.5M](figures/GSEA(1.5)M_dotplot.png)

### 2. Phase II: Metabolic Collapse & Scarring (6 Months)

Insight: The compensatory window closes. We observe a 93% directional reversal in the shared gene pool. The transcriptome is now defined by mitochondrial failure and reactive gliosis (scarring).

![Combined GO terms at 6M](figures/combined_ORAdotplots(6M).png)

![GSEA result at 6M](figures/GSEA(6M)_dotplot.png)

### 3. The "Biphasic" Transition
Insight: Comparing the two timepoints confirms the shift from neuroplasticity to neurodegeneration.

### Tech Stack & Methodology
This analysis was performed using R (v4.x) within a reproducible bioinformatics pipeline.

Differential Expression: limma, DESeq2

Functional Enrichment: clusterProfiler (GO, KEGG, GSEA)

Visualization: ggplot2, enrichplot, ggvenn

### Methodological Note
We specifically utilized GSEA over standard ORA (Over-Representation Analysis) to detect the sub-threshold metabolic shifts in the 1.5M dataset, demonstrating the utility of threshold-free methods in prodromal disease modeling.

### Contact
For inquiries regarding the code, collaboration, or the full manuscript, please contact:

Taye Motunrayo Ilesanmi Bioinformatician & Researcher
