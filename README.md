# Who-Painted-This
Final Project for Deep Learning Spring 2024
Link Google Colab Notebook: https://colab.research.google.com/drive/1__3GOuyrNr6Qvg3ENi6Qw7JPwZf-iicX?usp=sharing
Introduction Vincent Van Gogh, Salvador Dali, and Pablo Picasso painted thousands of works
between them and each claims to have been influenced by their predecessor. With similar yet
distinct styles drawing from each other, can a convolutional neural network learn to classify
these paintings by their artist?
Methods Paintings for each artist were downloaded from wikiart.com in batches. Around 770
images per artist, for a total of over 2,000 images in the dataset. Images were reviewed for
quality and accuracy, randomly shuffled, and split into a development and testing dataset
(80%/20% split). The development set was further split into a training and validation dataset
(80%/20% split). The images were resized, normalized and used to train convolutional neural
networks. Various architectures, parameters, and hyperparameters were trained and compared to
obtain the best fit model. Once a best fit model was trained, further experiments using
augmented data and regularization methods were performed to evaluate the impact on model
accuracy. Finally, a pre-trained model (Google’s Teachable Machine) was evaluated to determine
how it compared to the best fit model.
Results All three artists were evenly represented in the dataset, meaning the baseline accuracy
for this classification would be around 33.33%. The best fit model obtained 97.80% accuracy on
the test data set. Attempts to improve the model using data augmentation and regularization
methods did not result in improved accuracy on the validation dataset. Google’s Teachable
Machine was able to create a model which achieved between 81% and 89% accuracy between the
three classes.
Discussion A best fit convolutional neural network model was developed that could classify
paintings by artist with 97.80% accuracy on the test dataset. The baseline accuracy for this
dataset was 33.33% and the accuracy obtained by Google’s Teachable Machine ranged from
81%-89%, which indicates this is a highly accurate model
