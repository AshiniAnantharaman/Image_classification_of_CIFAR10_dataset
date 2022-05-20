# Image_classification_of_CIFAR10_dataset

The CIFAR-10 dataset contains 60,000 color images of 32 x 32 pixels in 3 channels divided into 10 classes. Each class contains 6,000 images. The training set contains 50,000 images, while the test sets provides 10,000 images.This is a classification problem with 10 classes(muti-label classification). We can take a view on this image for more comprehension of the dataset.

![CIFAR10_categories](https://github.com/AshiniAnantharaman/Image_classification_of_CIFAR10_dataset/blob/main/Dataset.png)

# More about the dataset

More details can be found in the below link.
https://www.cs.toronto.edu/~kriz/cifar.html

# Data lables using Categorical Encoding 

The output image class is categorically encoded with the values randing from 0 to 9.
The classes are:

Label	|Description|
------|------------
0	|airplane
1	|automobile
2	|bird
3	|cat
4	|deer
5	|dog
6	|frog
7	|horse
8	|ship
9	|truck

# Models involved

*   The classification is done using ANN.
*   The same classification is done using CNN as well.

- The results gathered by using an Artificial Neural Network is as below.
- Details of the neural network
  - Activation Functions: Sigmoid, ReLU
  - Loss: Categorical Cross Entropy
  - Optimiser: Adam
  - Metric: Accuracy
  - Epochs: 5

category |   precision |   recall | f1-score | support
---------|-------------|----------|----------|--------
0       |0.48      |0.55      |0.51      |1000
1       |0.63      |0.55      |0.59      |1000
2       |0.41      |0.20      |0.27      |1000
3       |0.32      |0.27      |0.29      |1000
4       |0.49      |0.26      |0.34      |1000
5       |0.37      |0.42      |0.40      |1000
6       |0.43      |0.60      |0.51      |1000
7       |0.44      |0.61      |0.51      |1000
8       |0.57      |0.62      |0.60      |1000
9       |0.51      |0.56      |0.54      |1000
accuracy      |          |          |0.47     |10000
macro avg      |0.47     |0.47     |0.45    |10000
weighted avg      |0.47     | 0.47    |0.45     |10000

- The results gathered by using a Convolutional Neural Network is as below.
- Details of the neural network
  - Activation Functions: ReLU, Softmax
  - Loss: Categorical Cross Entropy
  - Optimiser: Adam
  - Metric: Accuracy
  - Epochs: 5

category  | precision  |  recall | f1-score  | support
----------|------------|---------|-----------|--------
0     |  0.73   |   0.77    |  0.75  |    1000
1     |  0.84   |   0.78    |  0.81  |    1000
2     |  0.49   |   0.66    |  0.56  |    1000
3     |  0.51   |   0.52    |  0.51  |    1000
4     |  0.73   |   0.49    |  0.59  |    1000
5     |  0.61   |   0.53    |  0.57  |    1000
6     |  0.85   |   0.70    |  0.77  |    1000
7     |  0.66   |   0.81    |  0.72  |    1000
8     |  0.79   |   0.83    |  0.81  |    1000
9     |  0.76   |   0.80    |  0.78  |    1000
accuracy |      |          |  0.69   |  10000
macro avg |      0.70    |  0.69    |  0.69   |  10000
weighted avg   |    0.70    |  0.69    |  0.69 |   10000

# Results

As we can see, for the same number of epochs there is a huge change in Artificial and Convolutional Neural network.
The performance in the metrics like precision, recall, f1-score, etc. has increased for all the 10 categories.
