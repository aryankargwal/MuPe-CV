<div align='center'>

# MuPe-CV
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

</div>

## Abstract

Recently CNNs have become prevalent in garnering attention among students, developers and companies, due to their high predictive potential in various computer vision tasks, all the while dealing with high dimensional data involving thousands of classes. The idea of CNN, however, stems from Multi-Layer Perceptrons, something that drives the upcoming research work. <br>

In this context, we propose a comprehensive study of how MLP compares to modern CNN architectures in context to upcoming Computer Vision tasks that are the need of the hour. We provide the MLP of choice with an optimized network configuration and run it against a CNN architecture with similar variable and computational footing, giving accurate factors of the standings in Computer Vision tasks, namely Classification, Segmentation, and Detection. <Br>

The main motive behind this study is to explore networks with smaller footprints that can potentially achieve similar or slightly reduced accuracies to dense CNNs. This improves training, testing, and iteration time allows deployment of ML algorithms in IoT Devices to further ML on Edge development, lets these advanced architectures be used in parallel with computationally heavy tasks such as Virtual Reality or WebApp Development. <br>

## Dataset for the Tasks
[Fashion MNIST](https://github.com/zalandoresearch/fashion-mnistzzzzz): This dataset was used for this comparison due to the abundance of 28x28 pixel grayscale images which can be assigned to 10 classes and following the traditional MNIST dataset serves as a very accurate way to compare the performances of CNNs and MLPs.

## Model Architectures for the Task
### MLP
For the multilayer perceptron implementation to Classify images we trained a network with the following specifications.
- Layers: 4 Layers
- Parameters: 400,906
- Epochs: 200 (but will terminate at no change to the loss)<br>

<img src="assets/mlp_class.png" width="1000">

### CNN
For the CNN implementation to classify the images we trained a network with the following specifications
- Layers: 4 Layers
- Parameters: 694,090
- Epochs: 200 (but will terminate at no change to the loss)<br>

<img src="assets/cnn_class.png" width="1000">

## Training Results
For both training, a condition of training stopping incase of no improvement to validation loss was put. When this condition triggers the model weights from the end of the best epoch are restored and mapped into the evaluation metrics. Let us take a look at the results:
### MLP
The training stopped at the 18th epoch with no improvement to the validation loss and the weights from the 13th epoch are restored being the best.

<img src="assets/mlp_epoch.png">

Given is the plot for the Model Accuracy and Model Loss:

<img src="assets/mlp_loss.png">

Given is the confusion matrix for the classification task:

<img src="assets/mlp_conf.png">

Given is the Classification Report for the task:

<img src="assets/mlp_rep.png">

## Models to Train

- [x] Neural Network Classification
- [ ] Neural Network Segmentation
- [ ] Neural Network Detection
- [x] MLP Classification
- [ ] MLP Segmentation
- [ ] MLP Detection