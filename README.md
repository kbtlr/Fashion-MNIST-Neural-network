# Fashion-MNIST-Neural-network

A deep learning project comparing neural network architectures for image classification on the Fashion-MNIST dataset.

## Project overview

This project combines:
- a baseline fully-connected neural network (FNN) for proof of concept
- a convolutional neural network (CNN) for improved spatial feature learning
- regularization techniques (dropout, batch normalization) to reduce overfitting
- hyperparameter tuning and model evaluation pipelines

The current structure allows training multiple architectures side-by-side and comparing their performance. Rather than following a single tutorial, the project experiments with different approaches to understand why certain architectures outperform others, not just achieve high accuracy.

To run training:
```bash
python train.py --model cnn --epochs 50
```

To evaluate and visualize results:
```bash
python evaluate.py --model cnn
```

## Current stack

### ML framework
- Python
- TensorFlow / Keras
- NumPy, Pandas

### Data handling
- Fashion-MNIST dataset (60,000 training, 10,000 test images)
- Data preprocessing and normalization

### Evaluation & visualization
- Scikit-learn (metrics, confusion matrices)
- Matplotlib (loss curves, accuracy plots)

## Features and intended direction

The project is designed to support:
- baseline FNN model (~93% accuracy on test set)
- CNN architecture (~96% accuracy with fewer parameters)
- regularization experiments (dropout and batch normalization impact)
- hyperparameter tuning (learning rates, batch sizes, layer sizes)
- training visualization (loss curves, validation accuracy tracking)
- model comparison and confusion matrix analysis

## To Do

Baseline FNN is trained and working. CNN model training is in progress—currently debugging overfitting on certain clothing categories (shoes, bags). 

Will complete CNN training and add data augmentation (rotations, shifts) before testing transfer learning approaches.
