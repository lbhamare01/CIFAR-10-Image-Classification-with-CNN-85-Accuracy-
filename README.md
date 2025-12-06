# Image Classification using CNN (From Scratch)

## Objective
To design and train a Convolutional Neural Network (CNN) from scratch to classify images into different categories without using any pre-trained models.

## Dataset
- Dataset: CIFAR-10
- Total Images: 60,000
- Training: 45,000
- Validation: 5,000
- Test: 10,000
- Image Size: 32x32 RGB
- Classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

## Model Architecture
- Convolutional layers with ReLU activation
- Batch Normalization after each convolution
- MaxPooling layers for downsampling
- Dropout layers to reduce overfitting (0.2–0.5)
- L2 weight regularization
- Final Dense layer with Softmax activation

Total Parameters: ~1.18 Million

## Training Details
- Optimizer: Adam
- Learning Rate: 0.0005
- Loss Function: Categorical Crossentropy
- Batch Size: 64
- Epochs: 30
- Data Augmentation: Rotation, shift, zoom, flip, brightness

## Evaluation Results
- Test Accuracy: **84.88%**
- Test Loss: **0.64**

Training and validation curves show stable convergence with no significant overfitting.

## Observations
- Data augmentation significantly improved generalization
- Batch normalization stabilized training
- Dropout reduced overfitting at deeper layers

## Future Improvements
- Add precision, recall, and confusion matrix
- Experiment with learning rate scheduling
- Train for more epochs (100+)



