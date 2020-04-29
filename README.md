# Fruit-Vegetable-Classifier
A classifier that distinguishes between 5 different kinds of fruits and 5 different kinds of vegetables. 

The Neural Network's architecture is: 
CONV2D(32) -> MAXPOOL -> CONV2D(64) -> MAXPOOL -> CONV2D(128) -> MAXPOOL -> CONV2D(128) -> MAXPOOL -> DENSE(512) -> DENSE(10)I

In the transfer learning model, the architecture uses InceptionV3:
mixed7 -> DENSE(1024) -> DENSE(10)

Credits to https://github.com/TheCodingMaestro for scraping the images off the Internet and providing the data.

Changes:
1. Changed the optimizer from RMSProp to Adam
2. Added more layers of convolutions and padding
3. Added L2,L1 regularization along with dropout.
4. Used InceptionV3 over resNet50

Results:
Own Model- Epochs:30,  acc: 0.7152,  val_acc: 0.6385
Transfer Learning - Epochs:20, acc: 0.9240, val_acc: 0.7441

Any more epochs could result in overfitting. To reduce the variance of the validation accuracy, improve regularization, vary data distribution.

Feel free to add more classes and improve the model further!
