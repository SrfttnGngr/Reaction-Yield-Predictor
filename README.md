# 🧪 AI-Powered Chemical Reaction Yield Predictor

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![Status](https://img.shields.io/badge/Status-Complete-green)

## 📌 Overview
This project applies **Deep Learning (NLP techniques)** to organic chemistry. It predicts the yield of Suzuki-Miyaura coupling reactions based on their chemical structure (SMILES strings). 

Using a **Gated Recurrent Unit (GRU)** neural network, the model "reads" the atoms and bonds of reactants, reagents, and ligands to predict the experimental outcome. The project also includes a **Virtual High-Throughput Screening tool** that automatically recommends the best conditions (Solvent, Ligand, Base) for a given reaction.

## 🚀 Key Features
* **SMILES Tokenization:** Custom regex-based tokenizer to process chemical strings at the atom level.
* **Deep Learning Model:** A 2-layer GRU with Embedding and Dropout layers, implemented in PyTorch.
* **Reaction Optimization:** An algorithm that generates hundreds of "virtual experiments" to find optimal reaction conditions.
* **High Accuracy:** Achieved an **$R^2$ score of 0.852** and a Mean Absolute Error (MAE) of **~7.8%**.

## 🔬 The Science
The model treats chemical reactions as a "translation" problem. 
1.  **Input:** Reaction components are converted to SMILES (Simplified Molecular Input Line Entry System).
2.  **Embedding:** Atoms (C, N, O, Pd, etc.) are converted into dense vector representations.
3.  **Sequence Modeling:** The GRU reads the sequence of atoms to understand the chemical environment (sterics, electronics).
4.  **Output:** A predicted yield percentage (0-100%).

## 🛠️ Installation & Usage

1. **Clone the repository**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Reaction-Yield-Predictor.git](https://github.com/SrfttnGngr/Reaction-Yield-Predictor.git)
   cd Reaction-Yield-Predictor