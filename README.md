# Fraud Detection with Deep Learning
This repository contains the results of my teams experiments applying feedforward and autoencoder artificial neural networks toward mobile payments fraud detection. Our team was inspired by an academic paper, Fraud Detection using Machine Learning Techniques, written by Jurriaan Besenbruch (2018). A copy of this paper is included in this repository. Our team replicated the deep learning models examined in the paper and tried using random undersampling and synthetic minority oversampling techniques to determine which approach was best.

## Team Members
* [Yoseph Zuskin](https://www.linkedin.com/in/yoseph-zuskin/)
* [Krithika Shankar](https://www.linkedin.com/in/krithikashankar/)
* [Khalid Askar](https://www.linkedin.com/in/khalidaskar/)
* [Vicky (Xiaoqi) Ma](https://www.linkedin.com/in/vickyma20/)
* [Tokey (Mingzhong) Li](https://www.linkedin.com/in/tokeyli/)

## Data Source
Our team used the [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ntnu-testimon/paysim1) available on Kaggle (download by [clicking here](https://www.kaggle.com/ntnu-testimon/paysim1/download/WFkgBkx3T4g8fI1piSWE%2Fversions%2FaqkdOl5xmdvn6maMN5bg%2Ffiles%2FPS_20174392719_1491204439457_log.csv?datasetVersionNumber=2)).

## Summary of Findings
Surprisingly, our team determine that the best experiment we ran was actually the first one, which used a training subset of the unbalanced dataset with standardized scaling to fit a simple feedforward artificial neural network. The reason for such a conclusion is that, despite the true-positive percentage rate only being around 30%, the actual number of false-positive predictions when evaluating the model on the test subset of the data was the smallest from all the experiments. That means that if such a model were implemented, it would result in around 500 true-positive fraud detections for every false-positive. The low false-positive percentage rate from other experiments could be somewhat decieving as it ignored the fact that the dataset is extremely unbalanced, so every 0.5% to 2% false-positive percentage rates could mean thousands of false-positive classifications for only a few hundred true-positive classifications.
