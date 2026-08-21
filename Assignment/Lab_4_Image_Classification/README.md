# Image Classification and Recognition using R

## Objective

To implement a basic image classification and recognition system using R, EBImage, Keras3, and TensorFlow by following the prescribed tutorial.

## Reference

YouTube Tutorial: Image Classification & Recognition with Keras

## Dataset

The dataset contains 12 images:

- 6 images from class P (`p1.jpg` – `p6.jpg`)
- 6 images from class C (`c1.jpg` – `c6.jpg`)

The images are resized to `28 × 28 × 3` and reshaped into 2352 features.

## Libraries Used

- R
- EBImage
- Keras3
- TensorFlow

## Implementation

The following steps were performed:

1. Loaded and explored images.
2. Resized images to 28 × 28.
3. Reshaped images into feature vectors.
4. Created training and testing datasets.
5. Applied one-hot encoding.
6. Created a sequential neural network.
7. Compiled and trained the model for 30 epochs.
8. Evaluated the model.
9. Generated predictions and a confusion matrix.

### Model

2352 Input Features
        ↓
Dense(256, ReLU)
        ↓
Dense(128, ReLU)
        ↓
Dense(2, Softmax)

Results
- Training Accuracy: 100%
- Test Accuracy: 100%
- Training Images: 10
- Testing Images: 2
Test Confusion Matrix:
         Actual
Predicted 0 1
        0 1 0
        1 0 1
Files
- image_classification_with_r.ipynb – Google Colab implementation
- image_classification.R – R source code
- images.zip – Dataset
- confusion_matrix.csv – Confusion matrix result
- image_classification_model.rds – Saved model
- training_history.rds – Training history

Conclusion
The image classification implementation was successfully completed in R. The model correctly classified both test images in the provided dataset.
