# Fruit-Vegetable-Classifier
A classifier that distinguishes between 5 different kinds of fruits and 5 different kinds of vegetables. 

The Neural Network's architecture is: 
CONV2D(32) -> MAXPOOL -> CONV2D(64) -> MAXPOOL -> CONV2D(128) -> MAXPOOL -> CONV2D(128) -> MAXPOOL -> DENSE(512) -> DENSE(10)I

Credits to https://github.com/TheCodingMaestro for scraping the images off the Internet and providing the data.

Changes:
1. Changed the optimizer from RMSProp to Adam
2. Added more layers of convolutions and padding
3. Added L2,L1 regularization along with dropout.

Feel free to add more classes and improve the model further!
