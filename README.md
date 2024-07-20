# Using_DLModels_For_Leaf_Disease_Prediction
Deep learning uses artificial neural networks to perform sophisticated computations on large amounts of data. Deep learning algorithms train machines by learning from examples. Industries such as health care, eCommerce, entertainment, and advertising commonly use deep learning.

### Leaf Disease Detection Using Deep Learning Architectures

This project involves the implementation and comparison of four different deep learning architectures—GoogLeNet, VGG16, a custom Convolutional Neural Network (CNN), and VGG19—for the detection of leaf diseases. Each notebook follows a structured approach to achieve this goal:

1. **Data Preparation:**
   - The datasets are loaded and preprocessed using `ImageDataGenerator` from Keras, which includes augmentations like zooming, shearing, and horizontal flipping.
   - The dataset is downloaded from Kaggle and organized into training and validation sets.

2. **Model Building:**
   - **GoogLeNet, VGG16, and VGG19:** These models are loaded with pre-trained weights from ImageNet. Custom dense layers are added on top of the base models to adapt them for the leaf disease classification task.
   - **Custom CNN:** A custom architecture is built from using convolutional, pooling, and dense layers.

3. **Model Compilation:**
   - All models are compiled with the categorical cross-entropy loss function and accuracy as the metric.
   - Adam optimizer is used for training.

4. **Model Training:**
   - The models are trained using the training data, with validation data used for monitoring.
   - Early stopping and model checkpoint callbacks are employed to prevent overfitting and save the best model.

5. **Evaluation:**
   - The performance of the models is evaluated on the validation set, and accuracy and loss curves are plotted to visualize the training process.
   - The best model from each architecture is loaded for final evaluation.

6. **Prediction:**
   - The trained models are used to make predictions on test images, demonstrating their capability to classify various leaf diseases accurately.

### Results Summary

The performance of each model on the All Plant Diseases Dataset is summarized as follows:

1. **Custom CNN (different layers)**:
   - **Accuracy**: 94.04%

2. **VGG16 (modern CNN model)**:
   - **Accuracy**: 79.09%

3. **VGG19 (modern CNN model)**:
   - **Accuracy**: 78.28%

4. **GoogLeNet (modern CNN model)**:
   - **Accuracy**: 69.67%

These results indicate that the custom CNN model outperformed the pre-trained models (GoogLeNet, VGG16, and VGG19) in terms of accuracy on the leaf disease detection task.
