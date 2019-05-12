# Duo-ConvNet Dog VS Cat

This is a Conv model made with keras that can differantiate images of dogs and cats


## Installation

You can download or to clone this repository :

```sh
git clone https://github.com/kir486680/Duo-ConvNet.git
```

## Usage example

Classifier.py will tell you how to use the model !

## Model design

```
# Step 1 - Convolution
classifier.add(Conv2D(32, (3, 3), input_shape = (64, 64, 3), activation = 'relu'))

# Step 2 - Pooling
classifier.add(MaxPooling2D(pool_size = (2, 2)))

# Adding a second convolutional layer
classifier.add(Conv2D(32, (3, 3), activation = 'relu'))
classifier.add(MaxPooling2D(pool_size = (2, 2)))

# Step 3 - Flattening
classifier.add(Flatten())

# Step 4 - Full connection
classifier.add(Dense(units = 128, activation = 'relu'))
classifier.add(Dense(units = 1, activation = 'sigmoid'))
```


