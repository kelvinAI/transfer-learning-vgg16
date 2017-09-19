## Transfer Learning
In this guide we'll perform transfer learning using vgg16 on a different set of image data to perform image classification on it.
We'll use VGGNet trained on the ImageNet dataset as a feature extractor. Below is a diagram of the VGGNet architecture.
For transfer learning, all the convolutional layers are kept. We will replace the final fully connected layers with our own classifier.
By doing this VGGNet will become a feature extractor for our images and we can train a simple classifier on top of that using our own data. The first fully connected layer output from vgg16 has 4096 units, including thresholding with ReLUs. We can use those values as a code for each image, then build a classifier on top of those codes.

**Edited by**
- Kelvin Kong
