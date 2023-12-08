# Skin-Cancer-Classification-Ham10000-CNN---Data-Augmentation


![alt text](https://github.com/BheZelmat/Skin-Cancer-Classification-Ham10000-CNN---Data-Augmentation-/blob/main/img.png?raw=true)
## Project Overview
This project aims to leverage the power of Convolutional Neural Networks (CNNs) for the classification of skin cancer, utilizing the HAM10000 dataset. This rich dataset consists of dermatoscopic images of skin lesions, which are used to train a CNN model to distinguish between different types of skin cancer.

## Dataset
The HAM10000 dataset includes metadata for various skin lesions. Key columns in the metadata include:

lesion_id: Unique identifier for each lesion.
image_id: Unique identifier for each image.
dx: The diagnosis for the image (type of skin cancer).
dx_type: The type of diagnostic method used.
age: Age of the patient.
sex: Sex of the patient.
localization: The location of the skin lesion on the body.
dataset: The dataset source.
## CNN Model
We use a Convolutional Neural Network, a class of deep neural networks most commonly applied to analyzing visual imagery. The CNN will learn to identify patterns and features in the images that are indicative of various types of skin cancer.

## Data Augmentation
To address the issue of limited data and improve the generalization of our model, we implement data augmentation techniques. This involves artificially expanding the size of the training dataset by creating modified versions of the images. Techniques include rotations, zooming, shifts, shearing, and flipping. Data augmentation helps in reducing overfitting and improves model robustness.

## Usage
* Data Preprocessing: Load the HAM10000 dataset, preprocess the images, and split them into training, validation, and test sets.
* Data Augmentation: Implement data augmentation on the training set.
* Model Training: Train the CNN model using the augmented training data.
* Evaluation: Evaluate the model's performance on the test set.
* Prediction: Use the trained model to classify new skin lesion images.
## Dependencies
Python 3.x
TensorFlow
Keras
Pandas
Numpy
Matplotlib
How to Run
Detailed instructions on how to set up the environment, preprocess the data, train the model, and evaluate its performance are provided in the Notebook documentation.

## License
This project is open-sourced under the MIT license.
## Performance Metrics
* Testing Loss (Categorical Cross Entropy): Measures the performance of the classification model whose output is a probability value between 0 and 1. A lower loss indicates a better model. For this model, the testing loss is 0.706.

* Testing Accuracy: Represents the percentage of correct predictions out of all predictions made. The testing accuracy for this model is 75.0%. This means that 75% of the lesion images in the test set were correctly classified by the model.

* Testing Precision: Precision is the ratio of correctly predicted positive observations to the total predicted positives. High precision relates to a low false positive rate. The testing precision for this model is 81.0%.

* Testing Recall: Recall (Sensitivity) is the ratio of correctly predicted positive observations to all observations in the actual class. The testing recall for this model is 69.6%.

## Interpretation
The accuracy of 75.0% indicates a good level of reliability in the model's predictions. However, there is room for improvement, possibly through further tuning of the model or by using more complex architectures.
A precision of 81.0% suggests that when the model predicts a skin lesion as a specific type of cancer, it is correct 81% of the time. This is crucial for medical diagnostics to minimize false positives.
The recall of 69.6% shows that the model is somewhat conservative in its predictions, possibly missing some true positive cases. It’s important for medical applications to have a higher recall to ensure all potential cases are identified.
## Author 
- B Houssem E Zelmat 

