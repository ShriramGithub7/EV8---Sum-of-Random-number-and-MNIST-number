# EV8: Sum-of-Random-number-and-MNIST-number

This repository contains Neural Network code that takes 2 inputs and generate 2 outputs

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

**TRAINING LOGS:**

epoch: 0 total_correct: 50207 loss: 6101.303890347481 accuracy: 83.67833333333333
epoch: 1 total_correct: 57470 loss: 5639.896419167519 accuracy: 95.78333333333333
epoch: 2 total_correct: 58089 loss: 5599.023063659668 accuracy: 96.815
epoch: 3 total_correct: 58359 loss: 5581.097222805023 accuracy: 97.265
epoch: 4 total_correct: 58547 loss: 5569.991477251053 accuracy: 97.57833333333333
epoch: 5 total_correct: 58638 loss: 5564.482369184494 accuracy: 97.73
epoch: 6 total_correct: 58722 loss: 5558.712272286415 accuracy: 97.87
epoch: 7 total_correct: 58824 loss: 5552.5024873018265 accuracy: 98.04
epoch: 8 total_correct: 58797 loss: 5554.559280991554 accuracy: 97.995
epoch: 9 total_correct: 58803 loss: 5554.016873717308 accuracy: 98.005
epoch: 10 total_correct: 58777 loss: 5555.524003505707 accuracy: 97.96166666666667
epoch: 11 total_correct: 58887 loss: 5548.870395064354 accuracy: 98.145


