# Diabetic-Retinopathy-EyePACS

 Project Overview
The project follows a structured workflow:

Dataset Preparation:

Utilized the EyePACS and APTOS2019 datasets.
Preprocessing included CLAHE and Median Filter techniques for improved image clarity.
Image cropping and black background removal were employed to enhance focus on retinal features.

Data Handling:

Classes were merged into three categories:
Healthy
Early DR
Advanced DR
Images were split into 80% training and 20% validation for optimal model learning.

Data Augmentation:

Techniques like Horizontal/Vertical Flip, Random Brightness, and Gaussian Noise were applied using the Albumentations library.
Augmentation was heavily applied to address class imbalance.

Model Architecture:

Base model: EfficientNetB3.
Added layers:
Convolutional layers with swish activation.
Dropout layers to prevent overfitting.
Categorical Crossentropy with label smoothing for improved class distribution learning.

Training:

Optimizer: Adam with a learning rate of 0.0001.
Trained for 20 epochs with early stopping to prevent overfitting.

Evaluation Metrics:

Accuracy, F1-Score, and AUC.
Visualized performance using:
Confusion Matrix
ROC Curve
Occlusion Sensitivity Maps for interpretability.

📊 Results
Validation Set:
Accuracy: 86%
F1-Score: 84%
AUC: 93%
APTOS2019 Dataset:
Accuracy: 84%
F1-Score: 84%
AUC: 93%

Thus, achieving Generalization. 

