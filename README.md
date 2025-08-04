# anti-S. aureus Dataset

Introduction
-----------------------------------
anti-S. aureus-Dataset is the data set collected and curated from ChEMBL23 database for machine learning-based prediction models of anti-S. aureus activity.

We used an open-source software, AutoMolDesigner (V1.1) (https://github.com/taoshen99/AutoMolDesigner) , a new AI-based software for the design of small-molecule antibiotics developed by our research group, to construct classification models and applied this model to anti-S. aureus activity prediction of the compounds in the SPECS chemical library.

It was the first time that AutoMolDesigner was applied to real-world antibiotic discovery.

Dataset Description
-----------------------------------

SA_chembl2023.csv : S. aureus-related datasets (26,428 molecules) curated from ChEMBL23 database to build machine learning-based prediction models.
ag_train : ag_test = 8 : 2
Target prediction dataset : 1,212 highly potent anti-S. aureus compounds (MIC ≤ 0.1 μg/mL) were selected out from the dataset used for machine learning (SA_chembl2023.csv). 
