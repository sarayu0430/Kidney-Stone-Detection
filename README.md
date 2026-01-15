# Kidney Stone Detection (CT Image Classifier)

This project contains code and data organization for detecting kidney stones from CT images using a simple image classification pipeline and notebook-based experiments.

**Project layout**
- `Kidney_Stone_Detection.ipynb`: Main notebook with preprocessing, model training, and evaluation.
- `CT_images/`: Dataset root
  - `Train/`
    - `Normal/` (negative examples)
    - `Stone/` (positive examples)
  - `Test/`
    - `Normal/`
    - `Stone/`
- `Sample/`: additional example files

Getting started

1. Install Python 3.8+ and create a virtual environment:

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   pip install -U pip
   pip install -r requirements.txt  # if present
   ```

2. Open the notebook `Kidney_Stone_Detection.ipynb` in JupyterLab/Notebook and run cells top-to-bottom. The notebook expects the dataset to be organized under the `CT_images` folder as shown above.

Dependencies (typical)
- numpy, pandas
- matplotlib, seaborn
- scikit-learn
- tensorflow or torch (depending on which model approach you use)
- opencv-python or Pillow

Notes
- Ensure class folders contain the image files (PNG/JPG). Adjust file paths in the notebook if your dataset is located elsewhere.
- The notebook contains sections for data loading, augmentation, model definition, training, and evaluation — edit hyperparameters there.

