Neuroph works with JDK7 which is not available
Install JDK8 from https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
JDK12 tested but does not work.

Download from http://neuroph.sourceforge.net/download.html
neurophstudio-windows-2.96.exe

To create and train Perceptron neural network using Neuroph Studio do the following:
1. Create Neuroph Project.
2. Create Perceptron network. (from main menu choose File > New > Neural Network > Perceptron)
3. Create training set (from main menu choose File > New > Data Set)
4. Train network
5. Test trained network

#### Learning rate
During training, the backpropagation of error estimates the amount of error for which the weights of a node in the network are responsible. Instead of updating the weight with the full amount, it is scaled by the learning rate.
The learning rate is a configurable hyperparameter used in the training of neural networks that has a small positive value, often in the range between 0.0 and 1.0. Typical values for a neural network with standardized inputs (or inputs mapped to the (0,1) interval) are less than 1 and greater than 10^−6.<br />
The learning rate is often represented using the notation of the lowercase Greek letter eta (n).<br />
Generally, a large learning rate allows the model to learn faster, at the cost of arriving on a sub-optimal final set of weights. A smaller learning rate may allow the model to learn a more optimal or even globally optimal set of weights but may take significantly longer to train.<br />
potential issue: Oscillating performance, positive feedback<br />
solution: create a plot

#### Training epochs 
Passes through the training data

#### Momentum 
The amount of inertia of past updates is controlled via the addition of a new hyperparameter, often referred to as the “momentum” or “velocity” and uses the notation of the Greek lowercase letter alpha (a).
An exponentially weighted average of the prior updates to the weight can be included when the weights are updated. This change to stochastic gradient descent is called “momentum” and adds inertia to the update procedure, causing many past updates in one direction to continue in that direction in the future.
It has the effect of smoothing the optimization process, slowing updates to continue in the previous direction instead of getting stuck or oscillating.


