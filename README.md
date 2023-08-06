# X-ray Chest Disease Classification
This Jupyter Notebook presents my deep learning project for classifying X-ray chest images into four categories: Normal, COVID, Pneumonia, and Tuberculosis.

## Dataset
The dataset used for training and testing the model was meticulously collected from various reputable sources, including doctors' websites and Kaggle datasets. To ensure data quality, I performed data cleaning, meticulously removing duplicate images, and maintaining a high-quality dataset for training the model.

## Model Architecture
Model Architecture:
The CNN architecture comprises multiple convolutional layers with varying filter sizes and strides, enabling the model to learn hierarchical representations from the input images effectively. Max-pooling layers are strategically placed to downsample spatial dimensions and enhance feature extraction. The flattened output is connected to a series of dense (fully connected) layers, activated by Rectified Linear Units (ReLU) to introduce non-linearity. Dropout regularization is incorporated in the dense layers to prevent overfitting and enhance generalization. The final layer consists of four neurons with a softmax activation function, providing class probabilities for classification.

## Model Training and Evaluation
