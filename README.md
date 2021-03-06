# # 0x09. Transfer Learning

This project uses learning transfer with keras applications of the denseNet201 model to train convolutional neural networks to classify the CIFAR 10 data set.

## Requirements

 - `python3` (version 3.5)
 - `numpy` (version 1.15)
 - `tensorflow` (version 1.12)

## Files

It consists of two files:

**0-transfer.py**
It has a script that trains a convolutional neural network to classify the CIFAR 10 dataset and save trained model in the current working directory as `cifar10.h5`, making use of learning transfer from the denseNet201 model.
It also has the function `def preprocess_data(X, Y):`  that pre-processes the data for your model:
-   `X`  is a  `numpy.ndarray`  of shape  `(m, 32, 32, 3)`  containing the CIFAR 10 data, where m is the number of data points
-   `Y`  is a  `numpy.ndarray`  of shape  `(m,)`  containing the CIFAR 10 labels for  `X`
-   Returns:  `X_p, Y_p`
    -   `X_p`  is a  `numpy.ndarray`  containing the preprocessed  `X`
    -   `Y_p`  is a  `numpy.ndarray`  containing the preprocessed  `Y`

When you run the file it will look something like this:
 `$./0-transfer.py`
 
 ![image](https://user-images.githubusercontent.com/47121002/90203490-84c47a80-dda6-11ea-948a-5df2f312e14d.png)
 
 ...
 
 ![image](https://user-images.githubusercontent.com/47121002/90203685-fc92a500-dda6-11ea-9528-6c7475a25922.png)

**0-main.py**
It has a script to evaluate the model saved in the `cifar10.h5` file

## How to use it

 1. Clone the project
 2. Run the 0-transfer.py file, which will create a file called `cifar10.h5` with the trained network. This may take time.
 3. Run `0-main.py`to see network evaluation: loss and accuracy

## Author

* [**Ximena Carolina Andrade Vargas**](https://github.com/xica369)
is Backend, Mechatronic Engineer and Psychologist. She is a lover of Machine Learning.

	Twitter: @xica369
	LinkedIn: https://www.linkedin.com/in/xicav369/
	Project repository: https://github.com/xica369/0x09-transfer_learning/
	Blog: https://medium.com/@xica369/transfer-learning-6a7078a2f5fc
