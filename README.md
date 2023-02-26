# Pneumonia Detection

## Problem Statement:
X-rays aid doctor in determining the presence of pneumonia. To detect pneumonia, the radiologists commonly look for Infiltrates (an abnormal substance that accumulates gradually within cells or body tissues) indicating an infection. However, many images are affected by Low contrast, overlapping organs and blurred boundaries, as a result a highly accurate model is necessary.

## Model:
I used transfer learning, with the help of the famous ResNet50 model.

### Resnet-50:
The Resnet Artificial Neural Network is a deep feedforward neural network with 50 layers.

![Resnet](https://user-images.githubusercontent.com/62629426/221436198-ff4624a9-6a92-4186-81c9-39bfd1d73712.png)

Resnet uses Skip Connections, where a residual block takes in the output of a layer and forwards it to further layers. These skip connections are passed through parametric gates, which determine how much information passes through the skip connection, thus avoiding Vanishing and Exploding Gradients. They do that by acting as gradient super-highways, allowing it to flow without being altered by a large magnitude.

![Resnet Skip Connections](https://user-images.githubusercontent.com/62629426/221436479-23ce54c1-0c81-46b5-b617-fcf2a04d8f98.png)

As we can see, when new layers are added, the error decreases.

![Resnet accuracy](https://user-images.githubusercontent.com/62629426/221436677-e7411267-4f81-455a-a93d-51857c38006e.png)

For more information about Resnets check out this article (https://towardsdatascience.com/the-annotated-resnet-50-a6c536034758)

### Libraries: 
- [Tensorflow - Keras](https://www.tensorflow.org/api_docs/python/tf/keras)
- [tensorflow](https://www.tensorflow.org/)
- [Pathlib](https://docs.python.org/3/library/pathlib.html)
- [Matplotlib](https://matplotlib.org/)

### Results:
0: `normal`, 1: `Pneumonia `

### Accuracy:
- accuracy: 0.9250 
- Loss: 0.1472
