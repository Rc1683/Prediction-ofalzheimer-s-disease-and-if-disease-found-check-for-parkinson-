https://colab.research.google.com/drive/1ASIUzEBQjObhz2Q3MdUTdg1b1SLCDNj8?usp=sharing 
this is for parkinson model


Model Type: Uses MobileNetV2 for Parkinson's disease classification.
Data Handling: Utilizes ImageDataGenerator for data augmentation and loading images from a directory (/content/drive/MyDrive/new parkinson).
Model Architecture:
Loads a pre-trained MobileNetV2 model (with imagenet weights).
Adds a GlobalAveragePooling2D layer, followed by a dense layer with L2 regularization and dropout.
Uses a final dense layer with a sigmoid activation for binary classification.
Training Strategy:
Initially, the base MobileNetV2 model is frozen.
Uses binary_crossentropy loss and Adam optimizer.
Implements early stopping based on validation loss.
Applies class weighting to balance dataset classes.
Fine-tunes the model by unfreezing part of MobileNetV2.
Evaluation:
Generates predictions on validation data.
Computes an optimal decision threshold using ROC curve analysis.
Saves the trained model (parkinsons_mobilenetv2_finetuned.h5) and the optimal threshold (optimal_threshold.pkl).





https://colab.research.google.com/drive/1LcHvEflnbxBpb90HPkjdZVGh7BiBmHD4?usp=sharing
this is for Alzheimer's disease


Data Processing:

Reads oasis_longitudinal.csv and removes missing values.
Performs attribute selection using a statistical approach.
Feature Selection:

Implements forward and backward feature selection to find the most important attributes.
Model Training:

Uses K-Nearest Neighbors (KNN) and Support Vector Machine (SVM) for classification.
Data is standardized using StandardScaler before training.
Evaluation:
Computes accuracy scores for both KNN and SVM models.   

check if Alzheimer disease is present then Parkinson may come. I have done this also







/content/drive/MyDrive/new parkinson ](https://drive.google.com/drive/folders/1vOhZQwSPiv9j-VFb88lhB5y7qO3RIkNQ?usp=sharing)
dataset for parkinson



https://drive.google.com/drive/folders/1kUYxfWlQIIbpFkJbgSIbN5cM1I7OEisU?usp=sharing
dataset for alzheihmer




https://drive.google.com/drive/folders/1iEy5thIvy34Nfd4DXNvwsfNyHuwAwo9u?usp=sharing




pls follow the steps in code it will run succcesfully



for input take 1 test dataset for alzhemier disease and see the result
