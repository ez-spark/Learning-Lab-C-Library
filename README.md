<p align="center">
  <img src="https://i.ibb.co/bvbW4YL/photo2.jpg" alt="logo">
</p>

# Learning-Lab-C-Library:

Creating the library for Linux users:

```
sh create_library.sh
```

Compiling the tests for Linux users:

```
sh compile_tests.sh
```

# Current Roadmap:

- fully-connected-layers feed forward (20/11/2018)
- fully-connected-layers backpropagation (20/11/2018)
- nesterov momentum (20/11/2018)
- adam optimization algorithm (20/11/2018)
- fully-connected layers dropout (20/11/2018)
- convolutional layers feed forward (20/11/2018)
- convolutional layers backpropagation (20/11/2018)
- convolutional 2d max-pooling (20/11/2018)
- convolutional 2d avarage pooling (20/11/2018)
- convolutional 2d local response normalization (20/11/2018)
- convolutional padding (20/11/2018)
- fully-connected sigmoid activation (20/11/2018)
- fully-connected relu activation (20/11/2018)
- fully-connected softmax activation (20/11/2018)
- fully-connected tanh activation (20/11/2018)
- mse loss (20/11/2018)
- cross-entropy loss (20/11/2018)
- reduced cross-entropy form with softmax (20/11/2018)
- convolutional sigmoid activation (20/11/2018)
- convolutional relu activation (20/11/2018)
- convolutional tanh activation (20/11/2018)
- residual layers filled with convolutional layers (20/11/2018)
- residual layers feed-forward (20/11/2018)
- residual layers backpropagation (20/11/2018)
- model structure with fully-connected,convolutional,residual layers (20/11/2018)
- fixed residual issues (22/11/2018)
- adam algorithm for model_update (22/11/2018)
- size_of_model(model* m) function (23/11/2018)
- L2 Regularization (27/11/2018)
- Manual Batch normalization feed forward and backpropagation (27/11/2018)
- fixed residual issues2 (28/11/2018)
- Manual Xavier Initialization (28/11/2018)
- Clipping gradient (29/1/2019)
- Convolutional Layers with only pooling function (30/1/2019)
- Leaky Relu Activation function (30/1/2019)
- Batch Normalization final mean and variance for feed forward output (1/2/2019)
- Decision Tree structure (3/2/2019)
- LSTM feed forward (13/5/2019)
- LSTM back propagation (13/5/2019)
- Recurrent Network (rmodel) with LSTM (13/5/2019)
- Recurrent Network update with nesterov and adam algorithm (13/5/2019)
- Group Normalization for convolutional layers (4/7/2019)
- Residual LSTM cell (18/7/2019)
- Group Normalization for lstm layer (21/7/2019)
- Huber Loss (23/7/2019)
- Variational Auto Encoder for model structures (23/7/2019)
- VAE model feedforward and back propagation (23/7/2019)
- Modified Huber Loss (26/7/2019)
- Focal Loss (18/8/2019)
- Rectified Adam (22/8/2019)
- Gan model (28/8/2019)
- Confusion matrix and accuracy array (30/9/2019)
- KL Divergence (25/10/2019)
- Client-Server for distributed systems implementation (27/10/2019)
- Precision, Sensitivity, Specificity arrays (2/11/2019)
- NEAT algorithm (17/11/2019)

# Tests

Each test has been trained successfully.

The tests are trained on the CIFAR-10 Dataset that you can find in the data.tar.gz file, to run these tests you have to unpack data.tar.gz

- From test 1 to 6 there are different model* networks with different optimization algorithms, trained on supervised learning.
- Test 7 is a vae model trained on unsupervised learning.
- Test 8 is the test 6 trained on distributed systems client-server. To run it you have to connect 5 clients.
- Test 9 is trained with look ahead algorithm
- Test 10 is the Neat algorithm. it has been tested on the xor with the same parameter settings of the original paper:
  http://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf except for the feed forward (output node has a bias of 1) and the bias input node.
  Another difference is the removal connetcion rate. It has been set to 0.01 only if no connection has been added.
  However when a specie is close to the death (specie_rip param close to 15) then there is a change in the mutation behaviour:
  the add connection rate and removal connection rate are switched, in this case there is an inversion of the trend and the network
  try to simplify its structure. The test shows close results (even better) with the ones
  of the original paper. Indeed on 100 running test there is an avarage of 4680 total genomes computed, compared with the 4755 of the paper.
  But it needs more generations (an avarage of 41, propbably due to the offspring generation function) and in the worst case (33276 genomes computed).
  Pay attention the structure of the genome is different from the structure of the deep learning network.s
  The test 10 can be taken as neat template, you need only to change the compute fitness function


# Future implementations
- Variational auto encoder for rmodel* structure coming soon...
- ImageNet architecture coming soon...
- GAN for rmodel structure coming soon...

