# X-ray Chest Disease Classification
This Jupyter Notebook presents my deep learning project for classifying X-ray chest images into four categories: Normal, COVID, Pneumonia, and Tuberculosis.

## Dataset
The dataset used for training and testing the model was meticulously curated from reliable sources, including doctors' websites and Kaggle datasets. To ensure data quality, I performed rigorous data cleaning, meticulously removing duplicate images, resulting in a high-quality dataset suitable for training the model.
<br>
<br>
<p align="center">
    <img width="500" src="/figs/X-ray images.png" alt="Alt text" title="Optional title">
    <br>
    <em>X-ray chest images</em>
</p>
<br>
<br>
To tackle overfitting and enhance model generalization, I employed data augmentation techniques during the data preparation phase, diversifying the training data by applying random transformations to the images.

## Model Architecture
The heart of our X-ray Chest Disease Classification model lies in a robust Convolutional Neural Network (CNN) architecture. This architecture incorporates multiple convolutional layers with varying filter sizes and strides, enabling the model to learn hierarchical representations from the input images effectively. Max-pooling layers are strategically placed to downsample spatial dimensions and enhance feature extraction. The flattened output is connected to a series of dense (fully connected) layers, activated by Rectified Linear Units (ReLU) to introduce non-linearity. Dropout regularization is incorporated within the dense layers to prevent overfitting and improve generalization. The final layer consists of four neurons, each with a softmax activation function, providing class probabilities for accurate classification.

<p align="center">
    <img width="500" src="/figs/X-ray images.png" alt="Alt text" title="Optional title">
    <br>
    <em>X-ray chest images</em>
</p>

## Model Training and Evaluation
The model is trained using the carefully curated and preprocessed dataset, ensuring high-quality training data for optimal results. Prior to training, I split the dataset into training and validation sets, allocating 80% of the data for training and 20% for validation. The model was trained for 30 epochs, leveraging early stopping and the Adam optimizer. During the training process, I monitored the training and loss plots to identify any signs of overfitting. Based on the results, the model demonstrated exceptional performance, reaching a training accuracy of 0.9780 and a validation accuracy of 0.9494.
//

## Model Interpretability with Grad-CAM
In our X-ray Chest Disease Classification notebook, I ventured beyond model accuracy to explore model interpretability. Understanding the model's decision-making process is vital, and for this purpose, I adopted the Grad-CAM (Gradient-weighted Class Activation Mapping) technique.It provides valuable insights by highlighting the regions of X-ray images that significantly influence the model's predictions for specific classes.

///image

By leveraging the interpretability provided by Grad-CAM, we gain transparency into our model's reasoning, enabling us to validate its predictions.
