
# **MedMNIST Classification Using Deep Learning**

## **Overview**
This project focuses on classifying medical images from the **MedMNIST** dataset, specifically the **DermMNIST** dataset, using deep learning techniques. The goal is to build a model capable of classifying images of skin lesions into multiple categories based on dermatology-related conditions.

---

## **Dataset**
- **Source**: [MedMNIST Dataset](https://github.com/MedMNIST/MedMNIST)
- **Total Samples**: `10,015` images  
- **Classes**: 7 distinct types of skin lesions
  

## **Project Workflow**
1. **Data Preprocessing**  
   - The dataset is preprocessed by normalizing the image data for better model performance.  
   - The images are resized, and the dataset is split into **training (70%)** , **validation(10%)** and **testing (20%)** sets for model training and evaluation.

2. **Model Selection**  
   - The following models are used for classification:
     - **Custom CNN (Five Layers)**: A custom-built convolutional neural network with five layers.
     - **Pretrained ResNet**: A ResNet model, pretrained on ImageNet, used for transfer learning.
     - **Fine-Tuned ResNet**: A fine-tuned version of ResNet, sequentially trained on the DermMNIST dataset to enhance performance.

3. **Model Evaluation**  
   - The models are evaluated based on the **Accuracy Score** on the test and train dataset.

---

## **Results**
- The **Custom CNN** and **Pretrained ResNet** models were trained and evaluated on the DermMNIST dataset.
- The **Fine-Tuned ResNet model** outperformed the others, achieving an **accuracy of 73%** on the test dataset.
- The custom CNN and pretrained ResNet models provided reasonable results, but the fine-tuning of ResNet significantly improved the classification accuracy.
