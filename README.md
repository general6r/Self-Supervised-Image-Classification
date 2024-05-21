# Self-Supervised-Classification
 In this project, we implement the method discussed in this paper: "UNSUPERVISED REPRESENTATION LEARNING BY PREDICTING IMAGE ROTATIONS" (https://arxiv.org/pdf/1803.07728) 

Given the resource limitations, we won't be training the entire network from scratch. Instead, we'll be focusing on a subset of the models's weights. After that, we'll train the network on the CIFAR10 dataset for classification using the labels from the dataset(fully-supervised) and without the labels (self-supervised). The network architecture we'll be using is already implemented in PyTorch.

In essence, the network will learn to classify how each image has been rotated. After this training is performed, you can then fine-tune the supervised task. We'll be training a number of variations of the network (i.e. with / without this pre-training) and reporting results on each.

