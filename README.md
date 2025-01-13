In this project, we aim to classify plant diseases based on images of green leaves using deep learning techniques. We utilize a pre-trained ResNet model (Residual Networks), known for its effectiveness in image recognition tasks, to classify various leaf diseases. The model is trained on a custom dataset of images labeled with specific diseases that affect crops, helping to identify potential issues and guide appropriate interventions.

Objective:
The primary objective of this project is to build a robust image classification model that can automatically identify plant diseases from leaf images. By leveraging the power of ResNet, we aim to achieve high classification accuracy even with complex image features and variations. This can assist farmers and agricultural experts in early disease detection and help take preventive measures, thereby improving crop health and productivity.

Key Features:
Image Preprocessing:
The images are preprocessed to standardize their size and pixel values for feeding into the model. Images are resized to a consistent size (180x180 pixels) and normalized to a range of 0 to 1 for effective model training.

ResNet Model:
The ResNet model (typically ResNet-50, ResNet-101, or ResNet-152) is used as the backbone architecture for image classification. ResNet's key advantage lies in its deep residual connections that allow the model to learn more effectively, even with very deep networks.

Transfer Learning:
Transfer learning is employed by using a pre-trained ResNet model (pre-trained on ImageNet) and fine-tuning it for the specific task of leaf disease classification. This approach reduces training time and improves performance, especially when dataset sizes are limited.

Model Training:
The model is trained on a labeled dataset of plant leaf images, where each image corresponds to a specific plant disease or healthy leaf. The model learns to distinguish between these classes by extracting relevant features from the images.

Prediction and Evaluation:
After training, the model is capable of predicting the disease label for new leaf images. The performance of the model is evaluated using metrics like accuracy, precision, recall, and F1-score. Additionally, visualizations like confusion matrices and loss/accuracy plots are used to monitor training progress.

Technical Stack:
Programming Language: Python
Libraries and Frameworks:
TensorFlow/Keras (for model development and training)
Matplotlib (for visualizations and plotting)
NumPy (for numerical operations)
OpenCV (for image processing tasks)
Pandas (for data handling and manipulation)
Model:
ResNet (Residual Networks) – Pretrained on ImageNet and fine-tuned for plant disease classification.
Dataset:
The dataset consists of images of plant leaves categorized into different classes representing various diseases and healthy leaves. Each image is labeled with the respective disease, which may include common plant diseases like Potato Early Blight, Tomato Yellow Leaf Curl Virus, and others. The dataset is split into training, validation, and test sets.

Challenges:
Dataset Quality:
The quality and diversity of the dataset are crucial. A well-labeled, diverse dataset is necessary for the model to generalize well across different leaf types and diseases.

Overfitting:
Since the model uses a deep architecture (ResNet), there is a risk of overfitting to the training data. Techniques like data augmentation, dropout, and regularization are used to mitigate this issue.

Image Variability:
Leaves from different plants or under varying lighting conditions may appear different, leading to challenges in classification. Fine-tuning the model and using techniques like augmentation helps address this variability.

Conclusion:
This project demonstrates the potential of deep learning and the ResNet architecture for solving real-world agricultural problems. By automating the process of plant disease detection from leaf images, this system can aid farmers in early disease detection and intervention, ultimately contributing to better crop health management and enhanced agricultural productivity.

Future Work:
Model Optimization:
Further work can focus on optimizing the model for deployment in mobile applications or on embedded devices for real-time disease detection in the field.
 
Class Expansion:
The model can be trained with a larger and more diverse dataset, potentially covering a wider range of plant species and diseases to improve its generalization.

Integration with Agricultural Tools:
Integration of the model into existing agricultural tools or smartphones can help farmers in rural areas make faster, data-driven decisions about crop care.


**This is the fale result:**


 ![image](https://github.com/user-attachments/assets/2d6e2381-7ea1-47f7-a37a-69fb31c5f345)


 
**This is the example of True prediction** 



![image](https://github.com/user-attachments/assets/579d4bcd-e492-43a9-a8f0-a00e17d46fd9)
![image](https://github.com/user-attachments/assets/788be860-2dba-4e4d-8992-0c84f4e541c0)


