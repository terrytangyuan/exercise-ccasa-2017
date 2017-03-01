# CCASA 2017 TensorFlow Exercise

# Software Requirements

You need to have [Python](https://www.python.org/downloads/) and [pip](https://pip.pypa.io/en/stable/installing/) installed. Then install [TensorFlow](https://www.tensorflow.org/) via `pip install tensorflow`. Consult [this page](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/g3doc/get_started/os_setup.md) if you want to customize your setup. 

To test your installation, clone this repo and then run `python demo.py`. No error is expected if installation ws successful. You should expect the following at the end of the output:

```
Optimization Finished!
Accuracy: 0.9256
``` 

# Instruction

The Python script [demo.py](./demo.py) provides a basic example for logistic regression using TensorFlow on MNIST hand-written digit data. All the necessary steps, including data preprocessing, model building, and model evaluation, have been done for you so you can focus on small parts of the program. You are expected to make small modifications to the Python script [demo.py](./demo.py) to achieve the goals of the following exercises to get more familiar with TensorFlow's basics.

# Exercises

## Exercise 1: Minimize error using cross entropy as the cost function

* **Hint a:** Definition of [cross entropy](https://en.wikipedia.org/wiki/Cross_entropy) on Wikipedia. 
* **Hint b:** you'll need to use `tf.reduce_mean`, `tf.reduce_sum`, and `tf.log`.

## Exercise 2: Apply exponential learning rate decay

* **Hint a:** API Documentation for [Exponential Decay](https://www.tensorflow.org/api_docs/python/tf/train/exponential_decay). 
* **Hint b:** you can use `global_step = tf.Variable(0, trainable=False)` to initialize global step.

## Exercise 3: Achieve higher accuracy as much as possible (minimum 0.93)

* **Hint:** tune learning_rate, change optimizers, change cost function, more training steps, early stoping, etc.
