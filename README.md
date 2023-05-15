# Wheat disease detection
 
This is a Python script that implements a Convolutional Neural Network (CNN) model for detecting wheat diseases. It begins by importing necessary libraries and setting the paths for the dataset and images to be classified, which belong to 4 categories; healthy, leaf rust, crown and root rot, and loose smut. The dataset is loaded and preprocessed, converting the images into numpy arrays and normalizing their values. The data is then split into training and testing sets.

The CNN model is created using the Sequential model from Keras. It consists of multiple convolutional and max-pooling layers to extract features from the input images, followed by dense layers for classification. The model is compiled with appropriate settings such as optimizer, loss function, and accuracy metric. Data augmentation is applied to the training images using the ImageDataGenerator class from Keras, which introduces random transformations to increase the diversity of the data. The model is trained using the augmented data and the fit() function. After training, the model's performance is evaluated using the testing set. The accuracy and loss values are displayed.

The model is then used to classify new images by preprocessing them and predicting their labels. The predicted labels, along with the corresponding image names, are printed.

Finally, the trained model is saved in the H5 format for future use.
