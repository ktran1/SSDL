# SSDL
Semi-Supervised Dictionary Learning with graph regularized and active points (SSDL-GA)

This is an implementation of paper " SEMI-SUPERVISED DICTIONARY LEARNING WITH GRAPH REGULARIZED AND ACTIVE POINTS " Khanh-Hung TRAN, Fred-Maurice NGOLE MBOULA, Jean-Luc STARCK and Vincent PROST.

Require : sklearn, keras, scipy

Objective : We try to build the Dictionary learning model for classification objective that works for both limited number of labelled samples and limited number of unlabelled samples.  

For the MNIST database, we randomly select 200 images from each class, in which 20 images are used for labelled samples, 80 images are used for unlabelled samples and 100 images remain as testing samples.

For the USPS database, we randomly select 110 images from each class, in which 20 images are used for labelled samples, 40 images are used for unlabelled samples and 50 images remain as testing samples

Ladder is a semi-supervised neural network approach, implemented by "https://github.com/divamgupta/ladder_network_keras" can achive 98% with only 100 labelled samples and the whole disponible unlabelled samples (for MNIST). 

CNN is a simple convolutional neural network


| Method \ Data |   USPS       |      MNIST   |
| ------------- | ------------- | -------------|
| SSDL-GA       | 93.6 ± 1.0  |    90 ± 0.8      |
| CNN           | 89.28 ± 1.4  |     88.4 ± 1.1|
| Ladder        |  92.68 ± 1     |    89.84  ± 0.8      |

