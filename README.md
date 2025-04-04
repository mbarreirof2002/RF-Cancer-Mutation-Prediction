# RF-Cancer-Mutation-Prediction
An Interpretability-Focused Approach to Predicting the Effect of Cancer Mutations in Humans Using Random Forests


# 🧬 BIO_application – Cancer Mutation Classifier with Interactive Prediction

This notebook provides an interactive interface to explore and predict the pathogenicity of human cancer mutations using a pre-trained Random Forest model. It allows users to adjust mutation properties and immediately see how the model classifies the result as **Pathogenic** or **Benign**, along with a confidence score.

## 📋 What You Need Before Starting

To run this notebook, you'll need:

- The **trained Random Forest model** object (`best_random_forest.pkl`)
- The **processed DataFrame** (`cosmic_clinvar_processed.tsv`) used during model development (for medians and column structure)
- The **original DataFrame** (`cosmic_clinvar.tsv`) to train the LabelEncoder

These must be uploaded manually to Colab.

## 🚀 How to Use It

1. From the GitHub repository, download the following files:
   - `best_random_forest.pkl`
   - `cosmic_clinvar.tsv`
   - `cosmic_clinvar.tsv`
   - `BIO_application.ipynb`
     
   *The preview for BIO_applucation.ipynb is not available on GitHub*
3. Open [Google Colab](https://colab.research.google.com).
4. Go to **File > Upload Notebook**.
5. Upload the `BIO_application.ipynb` file.
6. In the **Files section** (left menu), upload the following files:
   - The trained model file (`best_random_forest.pkl`)
   - The original dataset (`cosmic_clinvar.tsv`)
   - The encoded dataset (`cosmic_clinvar.tsv`)
     
  *Wait for these to be fully uploaded before running the code!*
  
7. Run the notebook step by step.
8. Atlernativelly, you can go to **Runtime > Run all**.
9. Use the interactive interface to:
   - Type a gene name to search and encode it
   - Modify key mutation attributes (e.g., BLOSUM62 score, Hydrophobicity)
   - Select mutation type and somatic status
10. Click **Predict** to see the classification result and confidence.

## 💡 Features

- Built with `ipywidgets` for full interactivity
- Validates inputs (e.g., numeric ranges, gene validity)
- Uses dataset medians for features not set manually
- Visual and user-friendly: great for presentations and teaching!

## 🧠 Model Details

- Algorithm: Random Forest
- Trained on features including sequence context, biochemical impact, and mutation classification
- Output: Binary prediction (Pathogenic vs Benign) with confidence

---
