# anti-S. aureus Dataset

Introduction
-----------------------------------
* anti-S. aureus-Dataset is the data set collected and curated from ChEMBL23 database for machine learning-based prediction models of anti-S. aureus activity.

* We used an open-source software, AutoMolDesigner (V1.1) (https://github.com/taoshen99/AutoMolDesigner) , a new AI-based software for the design of small-molecule antibiotics developed by our research group, to construct classification models and applied this model to anti-S. aureus activity prediction of the compounds in the SPECS chemical library.

* Notably, this is the first time AutoMolDesigner has been applied to real-world antibiotic discovery!

Dataset Description
-----------------------------------

* S. aureus_chembl2023.csv (26,428 molecules)
  
   S. aureus-related datasets collected from ChEMBL23 database (https://www.ebi.ac.uk/chembl/) and curated by salt stripping, neutralization, SMILES standardization, the removal of compounds with too many rotatable bonds (> 20) and too high molecular weight (> 600) as well as the averaging of different MIC values for the same compound. Please note the compounds with average MIC below 32 μg/mL were defined as active compounds and the others were defined as inactive compounds. 

* S. aureus_train : S. aureus_test = 8 : 2 （randomly）

   These two files contain the compounds in the training set (21,142 compounds) and those in the test set (5,286 compounds) by random partion.  

* Target prediction dataset
  
   1,212 highly potent anti-S. aureus compounds (MIC ≤ 0.1 μg/mL) were selected out from the dataset used for machine learning (S. aureus_chembl2023.csv). 
