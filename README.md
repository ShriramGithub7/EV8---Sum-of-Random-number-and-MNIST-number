# EV8: Sum-of-Random-number-and-MNIST-number

**INPUT:**
  
This repository contains the code of model that will take 2 inputs:
  - image from mnist dataset that has number
  - random number between 0 to 9. 
 
 **OUTPUT:**
  
  Model is expected to generate 2 outputs:
  - number present in mnist image
  - sum of this mnist number and random number

**STRATEGY:**
  
Random number is generated using randint() function of random module in python3.

In the training network, few convolution layers are used for processing mnist image. Also few fully connected layers are used afte conv layers
Similarly, for random number, a fully connected layer is used in training.

Once both in inputs are passed through fully connected layers, their tensors are added together to get the sum.
cross_entropy loss function was used to calculate the loss.

**ACCURACY:**
  - Model is accurately able to find the number from MNIST dataset with quite good accuracy
  - sum of the mnist number and random number is not accurate

