# Algorithms For Massive Data
This repository contains Colab notebooks from Algorithms for Massive Data course at university of Milan. It contains both notebooks from laboratories and final project which is ocular disease recognition using the dataset provided by Kaggle: https://www.kaggle.com/andrewmvd/ocular-disease-recognition-odir5k



**Preprocessing Folder description**\
OCULAR_DISEASE_PREPROCESSING.ipynb - it is the first notebook that should be run. Firstly it downloads dataset from Kaggle. In order to successfully download the dataset via API, the kaggle.json file must be attached to the notebook files.  Notebook contains code for data preprocessing, resizing and creating validation set. All those operations are done once and then saved as a zip file in Google Drive. 

OCULAR_DISEASE_AUGMENTATION.ipynb - downloads preprocessed images from google drive and augments them by applying random zoom/rotations/brightness on minority classes. After applying augmentations it again saves the file to Google Drive.


**Training Folder description** - contains several experiments, each notebook trains the model  on a  different slice of the dataset.
OCULAR_DISEASE_RECOGNITION_N_C.ipynb - training the model to detect between normal fundus and cataract.

OCULAR_DISEASE_RECOGNITION_N_C_M.ipynb - training the model to detect between normal fundus, cataract, and myopia.

OCULAR_DISEASE_RECOGNITION_N_C_M_A.ipynb -  training the model to detect between normal fundus, cataract, myopia and AMD.

OCULAR_DISEASE_RECOGNITION.ipynb - train to detect all diseases (training performed on all data points).


**Laboratories folder** -  Not part of the project. Consist of files from course laboratories. 

