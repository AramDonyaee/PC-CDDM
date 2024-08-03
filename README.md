# Pancreatic-Cancer-Combinational-Analysis-GDSC2
Official codebase for pancreatic cancer combinational drugs analysis
### Original Dataset
The original dataset utilized in this study was obtained from Genomics of Drug Sensitivity in Cancer (GDSC2) combinations database. You can directly download the original dataset from [here](https://gdsc-combinations.depmap.sanger.ac.uk/downloads/pancreas/anchor_combo/). The original dataset is also available in this repository via `pancreas_anchor_combo.csv`.
### Calculated Molecular Descriptors
The original pancreatic cancer GDSC2 combinational dataset does not contain SMILES strings for the anchor and library drugs. Therefore, we have calculated the SMILES for the mentioned molecules with the help of PubChemPy python library. We then calculated the molecular descriptors for each unique molecule with PadelPy. The calculated descriptors for anchor and library drugs are stored in `anchor_descriptors.csv` and `library_descriptors.csv` files.
### Extended Dataset (Original + Molecular Descriptors)
After calculating the molecular descriptors, we then concatenated the descriptors files with the original dataset, extending it. The final dataset ready to go through pre-processing and model training is available from this [Google Drive link](https://drive.google.com/file/d/19XsxWVWBEihzLnyQ5GD1Xg7LZN1gsgJT/view?usp=sharing) The size of the dataset is close to 3 gigabytes.
### EDA (Exploratory Data Analysis) and Model Training.
Everything that is needed to replicate our study can be found in `pancreatic_cancer_combinational_ml.ipynb` jupyter notebook. The code for EDA, SMILES convertion, molecular descriptors calculation, pre-processing, model training, and model interpretation is accesible within the mentioned file.
