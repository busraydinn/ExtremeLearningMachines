This repository explains what an extreme learning machine is and its application areas.
# Extreme Learning Machines
Extreme Learning Machines are a type of single hidden layer feedforward artificial neural network model. They were introduced by Huang and colleagues in 2004. They use a Single Layer Feedforward Neural Network (SLFN) and compute the weights analytically after randomly assigning them, which accelerates the training process.
# ELM Architecture
ELM consists of three layers:</br>
* The input layer<br/>
* The hidden layer <br/>
* The output layer<br/>
![elm](https://github.com/user-attachments/assets/c4689442-03cf-48fd-9bcf-18f6adec2f89)

# The Input Layer
The input layer is the initial stage of the model where features from the external environment are introduced for processing. Each data sample is represented as a feature vector, serving as the input to the neural network.
<br/>
<h4>X=[x[1],x[2],....,x[N]]</h4>
<br/>

* The input is represented as a vector denoted by X.<br/>
* In this representation, each value in X corresponds to a specific feature or attribute of the data.<br/>
* N denotes the total number of features.<br/>

# The Hidden Layer
In ELM, the hidden layer weights (W) and biases (b) are randomly assigned and remain fixed during training, which distinguishes ELM from traditional backpropagation algorithms.
The number of hidden neurons is denoted by L. The greater the number of hidden neurons, the more complex the model becomes.<br/>

<h4>H=g(W*X+b)</h4><br/>

* H: Output of the hidden layer<br/>
* g: Activation function (e.g., ReLU, sigmoid, tanh)<br/>
* X: Input vector<br/>
* b: Bias<br/>
#The Output Layer
The output layer is the final layer that transforms the information from the hidden layer into the target outputs. In ELM, the output weights are computed analytically, meaning they are determined through a single mathematical operation.

The output predictions are denoted as f(x) and are calculated by multiplying the hidden layer output H with the output weights β (beta):<br/>
<h4>f(x) = H × β</h4><br/>
In ELM, the output layer weights are calculated using the Moore-Penrose pseudoinverse of the hidden layer output matrix. This output weight matrix is denoted by β (beta).<br/>

# Advantages:<br/>

* <h5>Very Fast:</h5> The training process is much faster compared to traditional methods.<br/>
* <h5>Easy to Use:</h5> It has a simple structure and is easy to configure.<br/>
* <h5>Strong Performance:</h5> It provides good results for most problems and is generally reliable.<br/>
* <h5>Clear Computation:</h5> It produces mathematically exact and repeatable results.<br/>
* <h5>Flexible Structure:</h5> It can be easily adapted to different problems and settings.<br/>

# Disadvantages:<br/>

* <h5>Random Results:</h5> Since the initial weights are randomly selected, the results may vary each time.<br/>

* <h5>Neuron Count Issue:</h5> Finding the correct number of neurons requires trial and error.<br/>

* <h5>Big Data Challenge:</h5> It uses a lot of memory for very large datasets and may slow down.<br/>

* <h5>Weak on Complex Problems:</h5> It may be insufficient in cases that require deep learning.<br/>

* <h5>Overfitting Risk:</h5> It may overfit on small datasets, learning too much from the data.<br/>



