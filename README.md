# S11

The model reaches a maximum accuracy of **92.26%**

### Parameters and Hyperparameters

- Loss Function: Cross Entropy Loss (combination of `nn.LogSoftmax` and `nn.NLLLoss`)
- Optimizer: SGD
  - Momentum: 0.9
  - L2 regularization factor: 0.01
- LR Range Test
  - Start LR: 1e-6
  - End LR: 0.02
  - Number of epochs: 10
  - Comparison Metric: Accuracy
- One Cycle Policy
  - Max LR: 0.02
  - Min LR: 0.002
  - Increase LR step size: 5 epochs
- Epochs: 24
- Batch Size: 512

### Data Augmentation

The following data augmentation techniques were applied to the dataset during training:

- Padding
- Random Crop
- Flip LR
- CutOut

