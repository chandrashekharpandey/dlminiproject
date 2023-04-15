# Deep Learning Mini Project

The aim of our project was to investigate the performance of RESNET-18 on the CIFAR-10 dataset with a parameter limit of less than 5 million.
As Neural Network research in image classification continues to flourish, larger corporations are developing "Very Deep Neural Networks" with hundreds of millions of parameters for high accuracy on ImageNet. However, training such models on smaller machines can be challenging. Therefore, we sought to determine whether a limited model size could achieve high accuracy. Our experiment focused on optimizing accuracy by exploring various attributes of the model. 
Our goal was to attain over 90% accuracy, and our best model was able to achieve 91.49% accuracy on CIFAR-10, meeting our expectations.

# Results

## Comparision with and without lookahead optimizer

| Optimizer | Learning Rate | Epochs | Batch Size | Test Accuracy|
| -------- | -------- | -------- | -------- | -------- |
| Adam with LookAhead | 1e-2 | 50  | 256 | 91.4|
| Adam without Lookahead| 1e-2 | 50 |256  | 90.72 |

## Comparision on batch size

| Optimizer | Learning Rate | Epochs | Batch Size | Test Accuracy|
| -------- | -------- | -------- | -------- | -------- |
| Adam  | 1e-2 | 50  | 128 | 91.11|
| Adam  | 1e-2 | 50  | 256 | 91.4|
| Adam  | 1e-2 | 50  | 512 | 91.2|

## Comparision on Learning Rate

| Optimizer | Learning Rate | Epochs | Batch Size | Test Accuracy|
| -------- | -------- | -------- | -------- | -------- |
| Adam  | 1e-1 | 50  | 256 | 89.90|
| Adam  | 1e-2 | 50  | 256 | 91.40|
| Adam  | 1e-3 | 50  | 256 | 90.95|

