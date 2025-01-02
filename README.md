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

## VISUALISE TRAINING SAMPLES
![image](https://github.com/user-attachments/assets/c94667ed-a280-4253-8dd7-121644d9e061)

## CNN ARCHITECTURE 
* Input Layer:  224x224 RGB images
* Three Conv Layer along with Maxpooling
  
  **Each Block:**
  - 1 Conv2D layer with 'relu' activation.
  - 1 MaxPooling2D layer.
* Flatten Layer
  - Two fully connected layer along with dropout
  - output layer with sigmoid activation function

 ![image](https://github.com/user-attachments/assets/7ca4112b-2b5b-42eb-8c4e-5495a7412168)

## MODEL COMPILATION AND TRAINING HYPERPARAMETERS
![image](https://github.com/user-attachments/assets/0ec3aaed-153f-41bd-beab-47bd27d29b1a)

## RESULT
**PLOT TRAINING AND VALIDATION ACCURACY AS WELL AS LOSS**
![image](https://github.com/user-attachments/assets/0f138924-438b-46d7-b882-b86bd31860be)

**TRAINING AND TESTING ACCURACY**
![image](https://github.com/user-attachments/assets/8aae7789-4ec6-455d-85d0-e3c4b1ab5056)

**CONFUSION MATRIX**
![image](https://github.com/user-attachments/assets/0ca1d970-fa2b-4d5a-92fa-b61f138b2e11)

## MODEL TESTING 
* Test the model on random unseen images.
* If fire is detected, trigger an alarm or notification system.


## Result:
![image](https://github.com/user-attachments/assets/b6ec607d-fb43-495a-a232-3e3f6018ad27)
![image](https://github.com/user-attachments/assets/334e27cb-095c-4ee7-acf2-c5b270f05b98)




## CONCLUSION
Using a CNN for the Early Fire Detection System leverages its strength in analyzing images to quickly and accurately identify signs of fire, such as smoke and flames. This enables real-time alerts, enhancing safety and response efforts. Proper training and optimization ensure the model is reliable and effective in various environments.

