

### Cross-sectional transcriptomic analysis of the retina in 5XFAD mouse model identifies stage-specific gene expression differences and candidate hub genes with potential biomarker relevance in AD
# Status: Paper Published (https://doi.org/10.1016/j.insi.2026.100404)  

---

## Abstract
Alzheimer's disease (AD) is the most prevalent form of dementia, with late diagnosis as a major contributor to its global burden. The retina, due to its physiological proximity to the brain, has been considerably studied as a potential site for early non-invasive AD biomarker changes. However, prior studies have been limited by single time-point design and the inability to identify specific genes associated with AD pathology in the retina. This study examined the retinal transcriptomic profiles of the 5xFAD mouse model through a cross-sectional analysis of RNA-sequencing data at early (1.5 M) and late (6 M) disease stages from the publicly available GSE274214 dataset, characterising stage-specific gene expression differences in retinal transcriptomic profiles at these two time points. Differential gene expression, functional and gene set enrichment, as well as Protein-Protein interaction analysis were performed to identify stage-specific transcriptomic signatures and hub genes. The cross-model expression overlap of the hub gene panel was then examined against an independent APP/PSEN1 dataset using PCA and ROC curve analysis. At 1.5 M, DEGs were predominantly enriched for synaptic signalling and neuronal pathways. While at 6 M, DEGs enrichment shifted toward mitochondrial dysfunction and glial activation, representing a pattern distinct from the early-stage profile. PPI analysis identified 20 hub genes associated with synaptic and mitochondrial activities, of which 16 were conserved in the APP/PSEN1 dataset and separated AD from wild-type samples in this small cohort (AUC = 1.0 in the 11-sample validation set); however, given the small sample size, this result should not be interpreted as evidence of diagnostic robustness. The findings of this study provide exploratory evidence of stage-specific gene expression differences in the 5xFAD retina and identify candidate hub genes warranting further investigation as molecular correlates of AD-associated retinal changes.


## Methodology
 Data Retrieval: Primary RNA-seq data (GSE274214) for 5xFAD and wild-type mice, alongside an independent validation dataset (GSE136861) for APP/PSEN1 mice, were retrieved from the NCBI GEO repository.  
#Differential Gene Expression (DGE): 
Raw read counts were converted to counts per million (CPM), filtered, and normalized using the TMM method. DGE analysis was executed within the R statistical environment using the limma package, applying the voom function to adequately model the mean-variance relationship.  
#Functional Enrichment: 
Gene Ontology (GO) and Gene Set Enrichment Analysis (GSEA) were conducted using the clusterProfiler package and fgsea algorithm to identify significant biological processes, cellular components, and molecular functions.  
#Network Analysis:
PPI networks were constructed via the STRING database and imported into Cytoscape for advanced topological analysis to extract the top highly connected hub genes for each temporal stage.  
#External Validation: 
Unsupervised Principal Component Analysis (PCA) via the prcomp function and Receiver Operating Characteristic (ROC) curve analyses were performed to evaluate the diagnostic variance and sample clustering efficacy of the identified hub genes.

## Key Findings
#Stage-Specific Perturbations: 
At the early 1.5-month stage, 470 DEGs were identified, predominantly enriched for synaptic signalling and neurodevelopment pathways. By the 6-month late stage, the profile underwent a metabolic shift, yielding 102 DEGs characterised by mitochondrial dysfunction, proton transmembrane transport, and glial activation.  
#Hub Gene Identification: 
PPI interactome analysis isolated 20 stage-specific candidate hub genes associated with vascular integrity, synaptic regulation, and mitochondrial activities.  
#Cross-Model Validation: 
16 of the 20 identified hub genes were successfully conserved in the independent APP/PSEN1 external validation dataset. These genes successfully segregated AD from wild-type samples, achieving perfect classification in the small validation cohort with an Area Under the Curve (AUC) of 1.0. 

## Tech Stack
Programming Language: R   
Transcriptomics & DGE Pipelines: *limma*, voom   
Pathway & Enrichment Analysis: clusterProfiler, fgsea   
Network & Interaction Biology: STRING Database, Cytoscape   
Statistical Modelling: prcomp (PCA), PROC package (ROC Curve Analysis)   
Data Visualization: ggplot2   

##Contact
For inquiries regarding the code, collaboration, or the full manuscript, please contact: motunrayoilesanmi85@gmail.com

Taye Motunrayo Ilesanmi Bioinformatician & Researcher
