<i>DISCLAIMER: This notebook was created solely for studying purposes, this must not be used for any real medical classification!</i><br><br>

# Breast-Cancer-Classification

I used transfer learning to classify benign and malignant images of breast cancer dataset. I used transfer learning as pre-trained InceptionResNetV2 with additional trainable Conv2D+DNN. During training i especially focused on recall metrics to evaluate model performance.


Used dataset: https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis/<br>
Useful link: https://towardsdatascience.com/convolutional-neural-network-for-breast-cancer-classification-52f1213dcc9

<b>Summary:</b><br>
- Dataset have been already labeled as benign or malignant<br>
- Images are loaded and based on its label (folder structure) we marked them as
  - Benign: 0
  - Malignant: 1
- Dataset is split as train set + test set
- Define and load ImageDataGenerator as setup data augmentation parameters
- Define and load pre-trained model InceptionResNetV2 + add additional trainable Conv2D and DNN layers
- Train model and make classification on test set
- Display metrics
