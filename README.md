# Evaluating Ensemble Methods for Glioma Classification
This Data Analysis project aims to identify gliomas as either LGG (Lower-Grade Glioma) or GBM (Glioblastoma Multiforme) through clinical and molecular/mutation factors, in order to minimize the number of molecular tests.  The data set is from the paper *Tasci, E., Zhuge, Y., Kaur, H., Camphausen, K., & Krauze, A. V. (2022). Hierarchical Voting-Based Feature Selection and Ensemble Learning Model Scheme for Glioma Grading with Clinical and Molecular Characteristics. International Journal of Molecular Sciences, 23(22), 14155* and is downloaded from https://archive.ics.uci.edu/dataset/759/glioma+grading+clinical+and+mutation+features+dataset.
## Variables: 
- Grade (Target variable): Glioma grade class information. (LGG, GBM)
- Gender
- Age at Diagnosis
- Race
- Project: Corresponding TCGA-LGG or TCGA-GBM project names.
- Case_ID: Related project Case_ID information.
- Primary_Diagnosis: Type of primary diagnosis information.
- IDH1: Isocitrate dehydrogenase 1 mutation status (NOT_MUTATED, MUTATED).
- TP53: Tumor protein p53 mutation status (NOT_MUTATED, MUTATED).
- ATRX: ATRX chromatin remodeler mutation status (NOT_MUTATED, MUTATED).
- PTEN: Phosphatase and tensin homolog mutation status (NOT_MUTATED, MUTATED).
- EGFR: Epidermal growth factor receptor mutation status (NOT_MUTATED, MUTATED).
- CIC: Capicua transcriptional repressor mutation status (NOT_MUTATED, MUTATED).
- MUC16: Mucin 16 mutation status (NOT_MUTATED, MUTATED).
- PIK3CA: Phosphatidylinositol-4,5-bisphosphate 3-kinase catalytic subunit alpha mutation status (NOT_MUTATED, MUTATED).
- NF1: Neurofibromin 1 mutation status (NOT_MUTATED, MUTATED).
- PIK3R1: Phosphoinositide-3-kinase regulatory subunit 1 mutation status (NOT_MUTATED, MUTATED).
- FUBP1: Far upstream element binding protein 1 mutation status (NOT_MUTATED, MUTATED).
- RB1: RB transcriptional corepressor 1 mutation status (NOT_MUTATED, MUTATED).
- NOTCH1: Notch receptor 1 mutation status (NOT_MUTATED, MUTATED).
- BCOR: BCL6 corepressor mutation status (NOT_MUTATED, MUTATED).
- CSMD3: CUB and Sushi multiple domains 3 mutation status (NOT_MUTATED, MUTATED).
- SMARCA4: SWI/SNF related, matrix associated, actin-dependent regulator of chromatin, subfamily a, member 4 mutation status (NOT_MUTATED, MUTATED).
- GRIN2A: Glutamate ionotropic receptor NMDA type subunit 2A mutation status (NOT_MUTATED, MUTATED).
- IDH2: Isocitrate dehydrogenase (NADP(+)) 2 mutation status (NOT_MUTATED, MUTATED).
- FAT4: FAT atypical cadherin 4 mutation status (NOT_MUTATED, MUTATED).
- PDGFRA: Platelet-derived growth factor receptor alpha mutation status (NOT_MUTATED, MUTATED).

## Implemented Models: 
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- Support Vector Machines
- k-Nearest-Neighbor

## Conclusion 
The k-Nearest Neighbors (kNN) model performs the best in terms of both AUC-score and Precision-score, demonstrating its strong capability to correctly classify the target variable. However, one limitation of kNN is that it does not provide a direct interpretation of feature importance, which makes it difficult to understand which variables are most influential in the classification process. 
On the other hand, Random Forest is the second-best model. It offers an important advantage in terms of feature importance, but has a lower AUC-score compared to kNN.
