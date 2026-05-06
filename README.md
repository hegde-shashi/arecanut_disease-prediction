# Arecanut / Betelnut Image Classification

This repository contains notebook-based image classification projects for arecanut and betelnut grading/disease prediction. The notebooks cover dataset loading, augmentation, model training, hyperparameter tuning, and evaluation with confusion matrices.

## Project Layout

- [betelnet_grouping/betelnut_grouping.ipynb](betelnet_grouping/betelnut_grouping.ipynb)
	- Betelnut grouping / grading workflow
	- Custom CNN training with hyperparameter tuning
	- MobileNetV2 transfer learning comparison

- [arecanut_disease_prediction/arecanut_disease_prediction.ipynb](arecanut_disease_prediction/arecanut_disease_prediction.ipynb)
	- Arecanut disease classification workflow
	- Custom CNN tuning and MobileNetV2 training
	- Validation and test-set confusion matrices

Model artifacts and tuner outputs are stored alongside each notebook.

## Environment

Recommended Python stack:

- TensorFlow 2.16.x
- tensorflow-metal for Apple Silicon GPU support
- keras-tuner
- numpy
- pandas
- matplotlib
- opencv-python
- scikit-learn

If you are using the `datascience` conda environment, verify TensorFlow and GPU access before running the notebooks.

## How To Run

1. Open the notebook you want to run in VS Code or Jupyter.
2. Update the dataset paths in the notebook to match your local machine.
3. Run the data loading, class inspection, and preprocessing cells first.
4. Run the custom CNN tuning/training cells.
5. Run the MobileNetV2 training and evaluation cells.
6. Review the confusion matrix and classification report outputs.

## Notes

- The notebooks are written to compare a custom CNN against MobileNetV2.
- Hyperparameter tuning outputs are saved under the local `*_tuning/` folders.
- Final trained models are saved as `.keras` files in the project folders.