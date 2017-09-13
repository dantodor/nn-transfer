# nn-transfer

This repository contains utilities for **converting PyTorch models to Keras**. More specifically, it allows you to copy the weights from a PyTorch model to an identical model in Keras.

From Keras you can then run it on the **TensorFlow**, **Theano** and **CNTK** backend. You can also convert it to a pure TensorFlow model (see [[1]](https://github.com/amir-abdi/keras_to_tensorflow) and [[2]](https://blog.keras.io/keras-as-a-simplified-interface-to-tensorflow-tutorial.html)), allow you to choose more robust deployment options in the cloud, or even mobile devices. Oh and from Keras you can also do inference in browsers with [keras-js](https://github.com/transcranial/keras-js).

*Keras -> PyTorch is not there yet: I am not sure whether there is any use case for that.*

## Installation
Clone this repository, and simply run

```
pip install .
```

You need to have PyTorch and torchvision installed beforehand, see the [PyTorch webiste](https://www.pytorch.org) for how to easily install that.

## Tests

To run the unit and integration tests:

```
python setup.py test
# OR, if you have nose2 installed,
nose2
```

There is also Travis CI which will automatically build every commit, see the button at the top of the readme.

## Code guidelines

* This repository is fully PEP8 compliant. I recommend `flake8`.
* It works for both Python 2 and 3.