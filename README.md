### MNIST Classifier Application: User Guide and Program Description

#### Program Overview:
The MNIST Classifier is a user-friendly application with a graphical interface built using PyQt5. It enables users to train a convolutional neural network (CNN) on the MNIST dataset and make predictions on hand-drawn digits. The application is powered by TensorFlow and Keras for model training and inference.

#### Key Features:
The program consists of three main sections:
1. **Main Menu** – The starting interface where users select training or testing options.
2. **Training Page** – Allows users to configure and train the CNN model.
3. **Drawing Page** – Users can draw digits and receive predictions from the trained model.

---

### User Guide:

#### Main Menu:
Upon launching the application, two options are available:
- **Train Model**: Opens the training page where users can configure and start training a model.
- **Test Model**: Navigates to the drawing page, allowing users to test the model (available only after a model has been trained or loaded).

#### Training Page:

##### Basic Settings:
- **Epochs**: Define the number of training epochs (range: 1-1000).
- **Batch Size**: Set the batch size for training (range: 1-1024).
- **Learning Rate**: Adjust the learning rate for the optimizer (range: 0.0001-1.0).
- **Optimizer**: Select the optimization algorithm (options: Adam, SGD, RMSProp).

##### Advanced Settings:
- **Data Augmentation**: Option to apply data augmentation techniques during training.
- **Learning Rate Schedule**: Enable to adjust the learning rate dynamically during training.
- **Early Stopping**: Stop training early if the model's performance plateaus.

Click **Start Training** to begin. Progress will be displayed with real-time updates on a progress bar, including training metrics. Upon completion, the option to save the trained model will be provided.

#### Drawing Page:
- **Draw**: Use the mouse to sketch a digit in the provided area.
- **Clear**: Erase the drawing to start over.
- **Predict**: The model will predict the digit, displaying the top 3 predictions along with their confidence levels.
- **Back to Main Menu**: Return to the main menu for additional tasks.

---

### Additional Information:
- The application automatically loads the last saved model on startup. 
- Users can train a new model or retrain an existing one anytime by visiting the training page.
- The drawing area features a 4x4 grid to assist with centering and sizing your digit.

This application provides an intuitive, interactive experience for training and testing neural networks on the MNIST dataset, allowing users to explore how well the model performs with their own hand-drawn digits.
