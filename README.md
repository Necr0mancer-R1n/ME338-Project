# ME338 Machine Learning Projects

This repository contains coursework projects for **ME338: Machine Learning for Engineering**.

The projects follow the course path from PyTorch basics to classical machine learning, neural networks, convolutional networks, and object detection. The main focus is to understand machine learning methods by implementing core components directly in Python and PyTorch.

## Setup

Install the required packages:

```bash
pip install torch torchvision matplotlib pillow wget notebook numpy scikit-learn
```


Then open the notebook for the project you want to run.

---

## Project 1: PyTorch Basics and KNN

This project introduces basic PyTorch operations and implements a K-Nearest Neighbor classifier.

Main topics:

* Tensor creation, indexing, slicing, and reshaping
* Broadcasting and batched matrix multiplication
* K-Nearest Neighbor classification
* Distance computation with two loops, one loop, and no loops
* Cross-validation for selecting `k`

Main files:

* `pytorch101.py`
* `pytorch101.ipynb`
* `knn.py`
* `knn.ipynb`

If CIFAR-10 is needed by the notebook, download it inside the Project 1 folder:

```bash
cd Project1
wget https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz
tar -xzf cifar-10-python.tar.gz
cd ..
```

---

## Project 2: Linear Classifiers and Two-Layer Neural Networks

This project implements basic image classification models from scratch.

Main topics:

* Multiclass SVM loss
* Softmax loss
* Naive and vectorized gradient computation
* Mini-batch stochastic gradient descent
* Hyperparameter search
* Two-layer fully connected neural network
* CIFAR-10 and MNIST classification experiments

Main files:

* `linear_classifier.py`
* `linear_classifier.ipynb`
* `two_layer_net.py`
* `two_layer_net.ipynb`
* `challenge_problem.ipynb`

Download CIFAR-10 inside the Project 2 folder:

```bash
cd Project2
wget https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz
tar -xzf cifar-10-python.tar.gz
cd ..
```

If the MNIST zip file is provided separately, extract it inside Project 2:

```bash
cd Project2
unzip mnist_dataset.zip
cd ..
```

---

## Project 3: Fully Connected and Convolutional Networks

This project builds deeper neural networks and convolutional networks using modular implementations.

Main topics:

* Fully connected networks
* ReLU, Dropout, and Batch Normalization
* SGD, Momentum, RMSProp, and Adam
* Naive convolution and max-pooling layers
* Three-layer ConvNet
* Deep ConvNet
* Kaiming initialization
* CIFAR-10 image classification

Main files:

* `fully_connected_networks.py`
* `fully_connected_networks.ipynb`
* `convolutional_networks.py`
* `convolutional_networks.ipynb`
* `p3_helper.py`

Download CIFAR-10 inside the Project 3 folder:

```bash
cd Project3
wget https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz
tar -xzf cifar-10-python.tar.gz
cd ..
```

---

## Project 4: Object Detection

This project implements object detection models on a tiny version of the PASCAL VOC 2007 dataset.

Main topics:

* RegNet backbone with Feature Pyramid Network
* FCOS one-stage detector
* Faster R-CNN style two-stage detector
* Region Proposal Network
* Anchor generation and box regression
* IoU and Non-Maximum Suppression
* Training and inference for object detection

Main files:

* `a4_helper.py`
* `common.py`
* `one_stage_detector.py`
* `one_stage_detector.ipynb`
* `two_stage_detector.py`
* `two_stage_detector.ipynb`

Download the VOC2007 dataset and annotation files inside the Project 4 folder:

```bash
cd Project4
wget https://web.eecs.umich.edu/~justincj/data/VOCtrainval_06-Nov-2007.tar
wget https://web.eecs.umich.edu/~justincj/data/voc07_train.json
wget https://web.eecs.umich.edu/~justincj/data/voc07_val.json
tar -xf VOCtrainval_06-Nov-2007.tar
cd ..
```

The object detection notebooks expect the following files to be available in the Project 4 folder:

```text
VOCdevkit/
voc07_train.json
voc07_val.json
```

---

## What I Learned

Through these projects, I practiced:

* Implementing machine learning algorithms from scratch
* Writing vectorized PyTorch code
* Training classifiers with gradient-based optimization
* Building neural networks with forward and backward propagation
* Understanding convolutional networks for image classification
* Implementing one-stage and two-stage object detection pipelines

---

## Acknowledgement

This repository was developed as part of **ME338: Machine Learning for Engineering**.
