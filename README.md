# nVidia Deep Learning Challanges Submission

## [https://drive.google.com/open?id=0B-A87zYQotkcQjhGQ3BFdUVtdWs](https://drive.google.com/open?id=0B-A87zYQotkcQjhGQ3BFdUVtdWs)

<p> please find code from google drive </p>

### Problem 1 - Creating Smarter and safer cities

### Problem 2 - AI in health care 

-------------------------------------------------------------------------

## Solution 1 - Developing Road Sign Classifier for city's neural network

<p>It will help machine brain to identify the meaning of road signs, So in smart citys it will give more experience for driverless cars and smart traffic control system. </p>


### Research Paper [Pierre Sermanet / Yann LeCun paper](http://yann.lecun.com/exdb/publis/pdf/sermanet-ijcnn-11.pdf)

### Architecture

<p>It is fairly simple and has 4 layers: 3 convolutional layers for feature extraction and one fully connected layer as a classifier</p>
<img src="https://navoshta.com/images/posts/traffic-signs-classification/traffic-signs-architecture.png"  height="200"/>

### Techniques Use

+ Dropout 
For every layer we need to calculate dropout.See in table given below : 
<pre><code>                Type           Size         keep_p      Dropout
 Layer 1        5x5 Conv       32           0.9         10% of neurons  
 Layer 2        5x5 Conv       64           0.8         20% of neurons
 Layer 3        5x5 Conv       128          0.7         30% of neurons
 Layer 4        FC             1024         0.5         50% of neurons
</code></pre>

+ L2 Regularization - We have to define lamda so we are *lambda = 0.0001* Which seems to perform the best.

+ Early stopping - We are using early stopping with a patience of *100 epochs*


### Training

We added two data sets to train our model

+ Pre Training
+ Fine Tuning 

### Visualization
+ Accuracy **97.05%**
+ Loss  **0.11%**

-----------------------------------------

## Solution 2 - Skin Cancer Classifier
<p>To explain AI in health care we implemented Skin Cancer classifier which can be used in heath care neural network.</p>

### Accuracy 70%



