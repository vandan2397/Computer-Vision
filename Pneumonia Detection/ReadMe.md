# PNEUMONIA DETECTION USING TRANSFER LEARNING

### Introduction
Pneumonia is a leading cause of morbidity and mortality in children younger than the age of 5 years, killing more children than HIV/AIDS, malaria, and measles combined.
Chest X-rays are primarily used for the diagnosis of this disease. However, even for a trained radiologist, it is a challenging task to examine chest X-rays. 
To solve the problem, we can use deep learning to extract hidden features, which are sometimes difficult to identify with naked eyes. Deep learning techniques can 
extract and can classify whether a patient has a Pneumonia or not and can save a lot of time of Radiologists. In this project, I have used deep learning techniques to detect 
Pneumonia from xray.

### Methods Used
- Data Augmentation
- Image Classification
- Deep Learning

### Tools and Libraries
- Python
- Pandas, Numpy, Matplotlib, Seaborn, Sklearn, and Keras
- Google Colab IDE

### Project Flow
<b>1) Data Collection</b>
  - Finding medical data is a challenging task. However, nowadays many open source platforms provide the medical data for research.
  - This data is collected from kaggle website (https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).
  
<b>2) Data Preparation/Augmentation</b>
  - Data augmentation can be very useful to avoid overfitting as it adds invariance in to the data and generates different images.
  - Here, I performed shear(0.2), rescaling, zoom(0.2), and Horizontal flip.

<b>3) Model Training</b>
  - Model training is also a crucial part, which helps to learn patterns or features within data.
  - In this project, I have used 4 different architectures to detect pneumonia in patient and compared their performances.
    - Basic Model with (3 convolutions and 3 pooling alternately)
    - VGG16 Architecture
    - RESNET Architecture
    - Inception net

<b>4) Perfomance Evaluation</b>
  - To evaluate the performance of different models, I have used precision, recall, and F1 score as the dataset is imbalanced.
  - Ratio of dataset was (Pneumonia-75) : (Normal-25)
  - ![Performance](https://user-images.githubusercontent.com/55615788/118265208-6f67b280-b4d6-11eb-8fe8-c3f10f483200.JPG)
  - From the above comparison, it can be concluded that VGG16 architecture outperfoms other architectures for this dataset.

<b>5) Deployment</b>
  - Using VGG16 model, build a flask app to deploy the model.
  - Results
  ![image](https://user-images.githubusercontent.com/55615788/118357994-63452900-b59a-11eb-9ead-9079747c1a22.png)
  
  
  
  
  




 
