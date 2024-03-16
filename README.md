# Slash-AI-task



1. **Data Preprocessing**: The code splits the dataset into training and validation sets using `splitfolders`. It then applies image augmentation techniques using `ImageDataGenerator` to enhance the variety of the training dataset.

2. **Model Creation**: I've designed a Convolutional Neural Network (CNN) model using TensorFlow/Keras' `Sequential` API. The model includes convolutional layers followed by max-pooling layers, a flattening layer, dropout layer for regularization, and dense layers for classification.

3. **Model Compilation**: I've compiled the model with the Adam optimizer and sparse categorical cross-entropy loss function.

4. **Model Training**: The model is trained using the `fit` method, with augmented training data and validation data, for a specified number of epochs.

5. **Observations and Issues**:
   - During training, the model encountered issues related to mismatches in convolution algorithms, likely stemming from differences in precision.
   - I noticed some warnings regarding XLA (Accelerated Linear Algebra) and cudnn (CUDA Deep Neural Network library), indicating possible compatibility or precision concerns.

6. **Overall Training Dataset Size**: I calculated the total number of images in the training dataset after augmentation.

7. **Visualization**: I visualized augmented and original images from the training dataset using Matplotlib.

8. **Results**: The code displays training progress, including accuracy and loss, for each epoch.
