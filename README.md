# Pneumonia-Detection

### Libraries: 
- [Tensorflow - Keras](https://www.tensorflow.org/api_docs/python/tf/keras)
- [tensorflow](https://www.tensorflow.org/)
- [Pathlib](https://docs.python.org/3/library/pathlib.html)
- [Matplotlib](https://matplotlib.org/)

### Data: https://www.dropbox.com/s/tlxserrdhe240lu/archive.zip

### Steps:
1. Import packages and load data
2. Getting directory path 
3. Split path to get label names
4. Split and train data
5. Create model, compile then fit

### Model:
I used transfer learning, with the help of the famous ResNet50 model

### Results:
0: `normal`, 1: `Pneumonia `

### Accuracy:
- accuracy: 0.9250 
- Loss: 0.1472
