# FlameShield-Smarter System for Early Fire Alerts
Early fire detection is crucial for minimizing damage and saving lives.  Traditional methods like smoke detectors and manual monitoring often suffer from delays and inaccuracies. Deep learning-based approaches offer real-time detection with higher precision, analyzing patterns from images and videos effectively.

## OBJECTIVE 
1. Develop advanced fire detection models using deep learning to detect and classify fire in diverse image scenarios.

2. Enhance model robustness by integrating diverse datasets and applying data augmentation techniques to improve performance across varying environmental conditions.

3. Implement a real-time alert system with an intuitive UI for instant fire alerts.

## PROBLEM STATEMENT  
Fires cause serious damage to people, property, and the environment. Traditional methods like sensors or manual checks are often slow and unreliable. A smart system using deep learning can help detect fires faster and more accurately, improving safety and response time.

## METHODOLOGY
![image](https://github.com/user-attachments/assets/c4d18658-581d-4a5f-8927-a87e748415b9)

## DATASET OVERVIEW
Data collected from Roboflow, total 4416 images divided into four classes. 
* url = { https://universe.roboflow.com/test-ojr0m/fire-detection-gj7u6 }
* publisher = { Roboflow }
* year = { 2024 }
* Roboflow Dataset Samples: 3198
* Extra Added Samples: 1218

## DATA PREPROCESSING
1. Resize Image: 224x224x3
2. Data Augmentation
   * rotation range
   * zoom range
   * width_shift_range
   * height_shift_range
   * horizontal_flip
   * brightness_range

## Visualise Training Images 
![image](https://github.com/user-attachments/assets/c94667ed-a280-4253-8dd7-121644d9e061)

## CNN ARCHITECTURE 
Input Layer:
  Size: 224x224 RGB images
Three Conv Layer along with Maxpooling.
             Each Block:
                        ￭  1 Conv2D layer with 'relu' activation.
                        ￭ 1 MaxPooling2D layer.
Flatten Layer
Two fully connected layer along with dropout
output layer with sigmoid activation function
1. Model Summary:
           Total Parameters: 11,177,281.

























### 9. Plot Training and Validation Accuracy/Loss
![image](https://github.com/user-attachments/assets/93236bb3-7923-46b0-9841-2ef6f5ecec74)

* Visualize the accuracy and loss curves for training and validation sets.
* Use Matplotlib to identify overfitting or underfitting.

### 10. Model Evaluation
![image](https://github.com/user-attachments/assets/03f9a16e-d177-48b8-9ed9-11098a5963b9)

* Evaluate the trained model on the test dataset.
* Generate metrics like accuracy, precision, recall, and confusion matrix.

### 11. Load Model for Predictions
* Save the trained model using model.save().
* Load the saved model for making predictions on unseen data.

### 12. Test the Model on Images
* Test the model on new images.
* If fire is detected, trigger an alarm or notification system.

____

## Result:

![image](https://github.com/user-attachments/assets/0323c2ab-d60e-4e29-98f4-e1cb60ca1ff4)


![image](https://github.com/user-attachments/assets/7debaf06-4351-42a0-9cca-aea605578a93)


![image](https://github.com/user-attachments/assets/fcbe0d6a-e21e-4268-a127-29f1426946e7)


![image](https://github.com/user-attachments/assets/1a216d57-8106-46f9-8e96-41ea28a34e0b)



