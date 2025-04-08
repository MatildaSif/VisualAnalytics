
# LEGO Brick Image Classification Using Pretrained CNNs

## Table of Contents
1. [Project Description](#description)
2. [Project Structure](#structure)
3. [Installation](#installation)
4. [Data Source](#data)
5. [Usage](#usage)
6. [Dependencies](#dependencies)
7. [Summary of outputs](#summary)
8. [Steps to Improvement](#improvement)

## Project Description
This project builds two convolutional neural network (CNN) models to classify LEGO bricks based on images. It uses a supervised machine learning approach, training on a labeled dataset from Kaggle.

Two CNN classifiers are implemented: one custom-built from scratch, and another leveraging feature extraction from a pretrained VGG16 model. The models are evaluated independently on test data using classification reports and plots of training loss and accuracy.

Results and visualizations are discussed and compared below, along with limitations and potential improvements.

## Project Structure
```
Assignment03/
│
├── src/
│   ├── CNN.py
│   └── VGG16.py
│
├── output/
│   ├── CNN_Classification_LossCurve.png
│   ├── CNN_Classification_report.txt
│   ├── VGG16_CNN_Classification_LossCurve.png
│   └── VGG16_CNN_Classification_report.txt
│
├── data/
│   ├── Cropped Images/
│   └── Base Images/
│
├── run.sh
├── setup.sh
├── requirements.txt
└── README.md
```

## Installation
To get started with this project, follow these steps:

1. unzip the folder called "Assignment03"
2. change directories into the  projects repository: /Assignment03
3. Follow the instructions under the Data Source section to collect the data
4. In the terminal, run `./setup.sh` to set up the Python virtual environment and install all dependencies.  
   - If you encounter a permission error, run `chmod +x setup.sh` and try again.
5. Run `./run.sh` to execute the training pipeline.
   - Adjust the script if you are using custom paths.
   - If you encounter a permission error, run `chmod +x run.sh` and try again

## Data Source
The data can be found at the link below:
https://www.kaggle.com/datasets/pacogarciam3/lego-brick-sorting-image-recognition

_Steps to download the data:_
1. Create a free profile on Kaggle
2. Click on the download button - choose download dataset as Zip
3. Unzip the data folder
4. Navigate into the general data folder
5. Add the "Cropped Images" and the "Base Images" folders directly into the "data" directory inside the "Assignment 03" folder. The final       structure will appear like thi:
    Assignment03/
    │
    ├── data/
    │   ├── Cropped Images/
    │   └── Base Images/


## Usage
Double check the folder_path and output_path (defined under the "Application" section of the main script)are set correctly based on your directory structure.
The output will be saved in the `output/` folder inside the `Assignment03` directory, unless a different output_path is defined.

## Dependencies
- `matplotlib==3.10.1`
- `re`
- `os`
- `numpy>=1.19.5mpy`
- `scikit_learn==1.6.1`
- `tensorflow==2.19.0`

## Summary of outputs

## Discussion of limitations

## Steps to Improvement


