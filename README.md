---
---



# Garbage Recognition with Deep CNN

This project implements a Convolutional Neural Network (CNN) for garbage image classification using a Kaggle dataset.

## Features

CNN model for image classification
Hyperparameter tuning
Evaluation of generalization performance




## Dataset

Due to its size the dataset is not included in this repository. 

This project downloads the dataset directly from Kaggle at runtime.

### Requirements

1. Create a Kaggle account.
2. Go to Kaggle Settings.
3. Under "Legacy API Credentials", click "Create Legacy API Key".
4. Download the generated `kaggle.json` file.

### Execution

When running the notebook, upload the `kaggle.json` file when requested. The dataset will then be downloaded automatically through the Kaggle API.

## Installation and Requirements

This project requires Python 3.x.

## How to run
Open the notebook in Google Colab.


## Project Structure

Amd_project_garbage_recogniser_DNN

└── LICENSE

└── .gitignore

└── Report

           └── images

           └── main.tex
           
└── notebooks
 

           └── garbage_cnn.ipynb

└── README.md



## Methodology


#### EDA
- Check dataset integrity: no duplicates or corrupted images,  consistent size/aspect ratio

#### Preprocessing
- Split dataset into train/validation/test
- Pixel normalization (division by 255)
- Data augmentation 

### CNN Training
- Hyperparameter tuning through Grid Search with K-Fold Cross Validation
- Final training using the best hyperparameters


### Model Evaluation
- Accuracy
- Training and validation loss curves
- Training and validation accuracy curves
- Confusion matrix
- Precision, Recall and F1-score


## Results

All the analysis and the results are contained in the file main.tex, for further informations about the CNN results refer to the uppersaid file. The entire project was implemented using a Mac device with a ninth generation Intel processor Core i7 6_core, so expect different running times if using different devices; the project was built to prioritize replicability and reasonable running time, less than an hour, rather than final accuracy.
So the goal of this project is not to achieve state-of-the-art performance, but to design, train and evaluate a complete deep learning pipeline while maintaining reproducibility and computational efficiency.

## Author
Samuele Magatti




## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
