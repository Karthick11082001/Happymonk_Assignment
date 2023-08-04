# Happymonk_Assignment
# Custom Activation Function for MNIST Digit Classification

This repository contains an implementation of an Artificial Neural Network (ANN) model using a custom activation function called `AdaActActivation` for digit classification on the MNIST dataset. The `AdaActActivation` is an adaptive activation function that enhances the learning capability of neurons.

## Dataset

The MNIST dataset consists of 28x28 grayscale images of handwritten digits from 0 to 9. It contains 60,000 training samples and 10,000 test samples. The data is preprocessed by scaling the pixel values to a range of [0, 1] and one-hot encoding the labels.

## Model Architecture

The ANN model is designed with the following layers:

1. Convolutional Layer: 32 filters of size (3, 3) with `AdaActActivation`.
2. MaxPooling Layer: Reduces spatial dimensions by (2, 2).
3. Flatten Layer: Converts the 2D feature maps into a 1D vector.
4. Dense Layer: 128 neurons with `AdaActActivation`.
5. Dropout Layer: A dropout rate of 0.5 is applied to reduce overfitting.
6. Dense Layer: Output layer with 10 neurons and `softmax` activation.

## Requirements

- Python 3.x
- TensorFlow 2.x
- NumPy
- Matplotlib

## Results

The model will be trained for 50 epochs, and the following results will be displayed:

- Final Parameter Values: `k0` and `k1` for the `AdaActActivation` function.
- Test Accuracy: Accuracy achieved on the test set.
- Test Loss: Loss value on the test set.
- F1-Score: Macro F1-Score on the test set.

A plot of the training and validation loss versus epochs will be shown, along with a classification report and confusion matrix.

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for improvement, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
