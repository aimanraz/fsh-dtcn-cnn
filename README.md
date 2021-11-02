# Fashion/Clothes Detection using Convolutional Neural Network (CNN)
Before we start, I want to share with you guys what inspired me to do this project, Did you guys know that according to the [news](https://economictimes.indiatimes.com/small-biz/sme-sector/fast-fashion-industry-wants-cheap-disposable-trendy-clothes-but-it-comes-at-a-price/articleshow/77032023.cms) in July 2020, fashion and textile industries contribute 2.3 % to the world GDP which equivalent to 1.8 trillion USD!. Yeah, textile and fashion industries under the major spotlight. Next, I want to share with you some old videos from YouTube about [Amazon 'echo look'](https://youtu.be/9X_fP4pPWPw) which also inspired me to develop this model.

## Code and Resources Used 
**Python Version:** 3.8++

**Packages:** pandas, numpy, sklearn, matplotlib, seaborn and tensorflow.

## Data collection and description
The dataset obtained from [SuperDataScience](https://www.superdatascience.com/courses) courses which also available on internet. Fashion training set consists of 70,000 images divided into 60,000 training and 10,000 testing samples. Dataset sample consists of 28x28 grayscale image, associated with a label from 10 classes, examples:

The 10 classes are as follows:  
0 => T-shirt/top
1 => Trouser
2 => Pullover
3 => Dress
4 => Coat
5 => Sandal
6 => Shirt
7 => Sneaker
8 => Bag
9 => Ankle boot

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255. 

## Visualization
Visualizing the flatten image.

![MNIST](https://github.com/aimanraz/fsh-dtcn-cnn/blob/main/img/Viz_dataset.png)

## CNN model
1. (32, 3, 2) kernel w/o dropout
2. (32, 3, 2) kernel with dropout 

## Model performance and Conclusion
* Advanced techniques using more rich dataset can be used to analyses the color, texture and style besides the categorical classification.
* There is slight increase in accuracy when using the dropout method. 

Some example visualization of the model prediction

![Prediction](https://github.com/aimanraz/fsh-dtcn-cnn/blob/main/img/viz_pred.png)

* (32, 3, 2) kernel w/o dropout:
    - Train accuracy: 94.42 %
    - Test accuracy: 91.30 %
 
* (32, 3, 2) kernel with dropout:
    - Train accuracy: 97.78 %
    - Test accuracy: 92.30 %

let the data drive you...and beyond.
