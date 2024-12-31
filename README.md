# FlameShield - Smarter System for Early Fire Alerts
## Overview:
Early fire detection is crucial for minimizing damage and saving lives.  Traditional methods like smoke detectors and manual monitoring often suffer from delays and inaccuracies. Deep learning-based approaches offer real-time detection with higher precision, analyzing patterns from images and videos effectively.
____
## OBJECTIVE 

### STEPS TO DEVELOP THE SYSTEM: 
**The project follows these detailed steps:**

### 1. Import Necessary Libraries
* Load essential Python libraries like TensorFlow, NumPy, Matplotlib, and OpenCV.
* Ensure all dependencies are installed using pip install -r requirements.txt.
### 2. Data Loading
* Load the image dataset containing Fire and Not-Fire classes.

**Split the dataset into training, validation, and test sets for model evaluation.**
### 3. Get Class Indices
* fire': 0, 'non_fire': 1
* Map the class names to numerical indices for model training and evaluation.
* Use TensorFlow/Keras utilities to generate class indices automatically.

### 4. Separate Labels from Test Set
* Extract image data and corresponding labels for the test set.
* Prepare the data for visualization and evaluation.

### 5. Visualize Training Images
![image](https://github.com/user-attachments/assets/dfcce7c3-b72f-4e4f-a1a3-b2c9baf6696b)

* Display sample images from the training dataset to understand the data distribution.
* Use libraries like Matplotlib for visualization.

### 6. Create Sequential Model
![image](https://github.com/user-attachments/assets/ffc22640-f532-4b09-a59a-b1568ee5ff4e)

* Define a CNN-based sequential model with layers for:
* Convolution and Max Pooling for feature extraction.
* Dense and Dropout layers for classification and regularization.

### 7. Compile and Train Model
* Compile the model using:
* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Metrics: Accuracy

### Train the model on the training dataset.

#### 8. Fit Model for Training
* Use the model.fit() function to train the model over multiple epochs.
* Monitor training and validation performance.

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

## Result:

![image](https://github.com/user-attachments/assets/0323c2ab-d60e-4e29-98f4-e1cb60ca1ff4)


![image](https://github.com/user-attachments/assets/7debaf06-4351-42a0-9cca-aea605578a93)


![image](https://github.com/user-attachments/assets/fcbe0d6a-e21e-4268-a127-29f1426946e7)


![image](https://github.com/user-attachments/assets/1a216d57-8106-46f9-8e96-41ea28a34e0b)



