# fasion-mnist-image-classification
Fashion MNIST image classification using an ANN

## Data description
Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes. Zalando intends Fashion-MNIST to serve as a direct drop-in replacement for the original MNIST dataset for benchmarking machine learning algorithms. It shares the same image size and structure of training and testing splits.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255. The training and test data sets have 785 columns. The first column consists of the class labels (see above), and represents the article of clothing. The rest of the columns contain the pixel-values of the associated image.

Labels

Each training and test example is assigned to one of the following labels:

    0 T-shirt/top
    1 Trouser
    2 Pullover
    3 Dress
    4 Coat
    5 Sandal
    6 Shirt
    7 Sneaker
    8 Bag
    9 Ankle boot
    
## Task
Without changing Neural Network architecture reach accuracy on test dataset>= 90%. (i.e. model must contain only 3 trainable layers and they must be Fully Connected (Dense), but we can add non-trainable parameters, decrease neurons number)

Also, some requirenments should be fullfilled:
* create evaluation function to calculate accuracy for this classification problem;
* create custom `loss_function(y_true, y_pred)`;
* it is prohibited to use: `model.fit(...)` and `tf.keras.optimizers` (but it is allowed to inherit from `tf.optimizers.Optimizer` and write our own optimizer)

## Result
All requirenments were fullfilled, the desired accuracy rate was reached:

` Test accuracy of the base model: 0.9009000062942505`
