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
  
-Random number is generated using randint() function of random module in python3.

-In the training network, few convolution layers are used for processing mnist image. Also few fully connected layers are used afte conv layers
Similarly, for random number, a fully connected layer is used in training.

- Once both in inputs are passed through fully connected layers, their tensors are added together to get the sum.
- cross_entropy loss function was used to calculate the loss.
- training is performed on CUDA (GPU)

**ACCURACY:**

  - Model is accurately able to find the number from MNIST dataset with quite good accuracy
  - sum of the mnist number and random number is not accurate

**TRAINING LOGS:**

epoch: 0 total_correct: 53918 loss: 5875.4244730472565 accuracy: 89.86%

epoch: 1 total_correct: 57787 loss: 5619.52460193634 accuracy: 96.31%

epoch: 2 total_correct: 58223 loss: 5590.693505764008 accuracy: 97.04%

epoch: 3 total_correct: 58447 loss: 5575.756269693375 accuracy: 97.41%

epoch: 4 total_correct: 58533 loss: 5570.622574925423 accuracy: 97.56%

epoch: 5 total_correct: 58572 loss: 5567.908988595009 accuracy: 97.62%

epoch: 6 total_correct: 58648 loss: 5563.639644503593 accuracy: 97.75%

epoch: 7 total_correct: 58656 loss: 5562.603075265884 accuracy: 97.76%

epoch: 8 total_correct: 58826 loss: 5552.839111566544 accuracy: 98.04%

epoch: 9 total_correct: 58780 loss: 5555.179874300957 accuracy: 97.97%

epoch: 10 total_correct: 58880 loss: 5549.132606506348 accuracy: 98.13%

epoch: 11 total_correct: 58729 loss: 5558.45803809166 accuracy: 97.88%
