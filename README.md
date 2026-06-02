# 🧬 Leprosy T1R Skin-Lesion Transcriptomics

**Repository:** `leprosy-t1r-skin-transcriptomics`

This repository contains the R analysis workflow and supporting files for the study:

**Integrated Skin-Lesion Transcriptomics Identifies Biomarker-Relevant and Pharmacologically Tractable Host-Response Axes in Leprosy Type 1 Reaction**

---

## 📌 Overview

Type 1 reaction (T1R) is an inflammatory complication of leprosy. This project analyses skin-lesion transcriptomic data to identify host-response genes and biological axes that distinguish **T1R_R1 reactional lesions** from **borderline non-reaction lesions**.

The analysis focuses on prioritising biologically interpretable T1R candidates using lesion-level expression, network support, immune-programme context, cross-dataset directionality and drug-target evidence.

---

## 🎯 Study focus

The repository supports the identification of:

* lesion-derived T1R host-response genes
* Tier 1 candidate biomarkers
* inflammatory and tissue-remodelling axes associated with T1R_R1 lesions
* drug-target-supported host-response candidates for future validation

---

## 📂 Public datasets

| Dataset       | Sample source | Role                                                                           |
| ------------- | ------------- | ------------------------------------------------------------------------------ |
| **GSE74481**  | Skin lesions  | Primary discovery dataset for T1R_R1 versus borderline non-reaction comparison |
| **GSE269151** | Whole blood   | Independent blood-ranked support for skin-derived T1R candidates               |

Both datasets are publicly available from the **Gene Expression Omnibus (GEO)**.

---

## 🧪 Analysis included

This repository includes scripts and processed outputs related to:

* skin-lesion differential expression analysis
* functional enrichment and immune-programme interpretation
* WGCNA and network-supported candidate prioritisation
* internal signature assessment
* cross-dataset blood-ranked support
* DGIdb and ChEMBL drug-target evidence mapping
* Cytoscape-ready network files for selected drug-target-supported candidates

---

## 🧩 Prioritised biological axes

The final Tier 1 candidate panel represents major T1R-associated host-response processes, including:

* myeloid and oxidative response
* cytokine and interferon signalling
* endothelial interaction
* leukocyte migration
* extracellular matrix remodelling

Representative candidates include **JAK2, ICAM1, TNF, FGR, CYBB, FN1, IL4R, PLAUR** and **CD40LG**.

---

## 💊 Druggability interpretation

DGIdb and ChEMBL were used to assess whether prioritised host-response candidates have existing drug-gene or target-level evidence.

These results provide **pharmacological context only**.
They should not be interpreted as treatment recommendations for leprosy Type 1 reaction.

---

## 🗂️ Repository contents

| Folder               | Description                                     |
| -------------------- | ----------------------------------------------- |
| `scripts/`           | R scripts used for data processing and analysis |
| `results/`           | Processed analysis outputs and summary tables   |
| `figures/`           | R-generated analytical figures                  |
| `tables/`            | Main and supplementary tables                   |
| `cytoscape_network/` | Node and edge files for network visualisation   |

---

## ⚙️ Software

The analysis was performed in **R** using standard CRAN and Bioconductor packages for transcriptomic analysis, enrichment, WGCNA, validation, visualisation and table generation.

Commonly used packages include:

```r
tidyverse
limma
edgeR
clusterProfiler
ReactomePA
WGCNA
pROC
randomForest
ggplot2
pheatmap
writexl
readxl
```

---

## 🎨 Figure preparation

Analytical plots were generated using R, and composite figures were assembled in Canva without changing the underlying data.

---

## 📬 Contact

For questions about this repository, please contact:

**Dr. Abida Khan**
Email: [aqua_abkhan@yahoo.com]

---

## ⚠️ Disclaimer

This repository provides computational analysis scripts and supporting files for research purposes only. Drug-target links reported in this work indicate existing database evidence and do not establish clinical efficacy, safety or treatment relevance in leprosy Type 1 reaction.
