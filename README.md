# Traffic Sign Recognition

This project is a deep learning model that uses convolutional neural networks (CNNs) to predict traffic signs. The model is trained on the German Traffic Sign Recognition Benchmark (GTSRB) dataset, which contains over 50,000 images of 43 different traffic signs.

## Requirements
- Python 3.5 or later
- TensorFlow 2.0 or later
- NumPy
- Matplotlib
- OpenCV (for image pre-processing)

or simply download all the files in the requirements.txt file [pip install -r requirements.txt]

## Getting Started

1. Clone this repository:

2. Download the GTSRB dataset from [here](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset) and extract it to the root directory of the project.
<!-- 3. Run the `preprocessing.py` script to resize, normalize, and convert the images to grayscale.
4. Run the `train.py` script to train the model. The script will save the trained model to the `models` directory.
5. Run the `test.py` script to evaluate the performance of the model on the test set. -->

## Model Architecture

The model architecture consists of the following layers:
- 2 convolutional layers with 32 filters each, kernel size of (3,3) and ReLU activation
- Max pooling layer with a pool size of (2,2)
- Dropout layer with a rate of 0.25
- 2 convolutional layers with 64 filters each, kernel size of (3,3) and ReLU activation
- Max pooling layer with a pool size of (2,2)
- Dropout layer with a rate of 0.25
- Flatten layer
- Fully connected layer with 512 units and ReLU activation
- Dropout layer with a rate of 0.5
- Fully connected layer with 43 units and softmax activation

## Results

The model achieved an accuracy of 99.2% on the test set.

## Note

This is a simplified version of a traffic sign recognition system, in real-world applications, more preprocessing and data-augmentation techniques should be applied, and more advanced architectures should be considered.

Feel free to use this code as a starting point for your own project and improve upon it.

## References
- [GTSRB dataset](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset)
- [Traffic Sign Recognition with Multi-Scale Convolutional Networks](https://ieeexplore.org/abstract/document/6909624)
