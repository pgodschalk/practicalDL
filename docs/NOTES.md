# Notes

## Neurons & Neuron Layers

- Data channel represented by
  $\mathrm{Neuron} = \sum_i {X_i}{W_i} + \mathrm{Bias}$ where
  $X = \mathrm{input signal}$ and $W = \mathrm{weight}$
- Neuring outputting boolean value based on activation
- [Sigmoid function](https://mathworld.wolfram.com/SigmoidFunction.html) to
  shrink the distribution of outputs to between 0 and 1

  ![Sigmoid function](static/image.png)

## Deep Learning

- Multiple layers to jump from linearity to more complex polynomials

## Neurons & Model Training

- Forward propagation: Random weights and biases during training
- Backward propagation: Compare result of forward propagation to original
  prediction and reinforce previously made correct decisions (by increasing
  weight or decreasing of each previous neuron through layers)
- Weight is calculated from the derivative

## Deep Learning & AI

- Recreation is the inverse operation of Deep Learning

## Learning Rate & Gradients

- Learning rate is a hyperparameter
- Hyperparameters control how training is happening
- Loss function is the measurement of the error
  - In a neural network, it's the measurement of if you did a correct
    prediction

## Sigmoid vs ReLU

- ReLU will set to 0 when signals are negative, returns value when positive
- $\mathrm{ReLU} = \max(x,0)$
- Regularization to not output too large values

## Softmax

- Softmax also outputs between 0 and 1, but guarantees that, with several
  units, the sum of all outputs is equal to 1
- This allows outputs from neurons to be viewed as probabilities
- Can be considered similar to `OneHotEncoding`

## Understanding the Model

- Dense layer: each neuron connected to every other neuron in the next layer

## Defining the Solver & Loss Function

- Earlier linear regression similar to stochatic gradient descent: started with
  a random point and gradually descended through gradient space to get to the
  extrema of the function

## Training a Model

- Epochs: number of times the model will see the entire dataset


## Comparing Different Models

- Add a validation set which models have never seen before (not part of
  training or validation data set)
