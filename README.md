# CIFAR-10-Object Recognition in Images

* Question: Identify the subject of 60,000 labeled images?

<!--- <img src="https://github.com/ChenghaoDing90/CIFAR10/tree/main/result/snapshot.png" alt="Dataset" style="width: 400px;"/> --->
<!--- ![ScreenShot](/result/snapshot.png width="100" height="100")  --->

<img src="./result/snapshot.png" alt="The first 36 images" style="width:300px;height:300px;" />

CIFAR-10  is an established computer-vision dataset used for object recognition. It is a subset of the 80 million tiny images dataset and consists of 60,000 32x32 color images containing one of 10 object classes, with 6000 images per class.

## Data Description
The CIFAR-10 data consists of 60,000 32x32 color images in 10 classes, with 6000 images per class. There are 50,000 training images and 10,000 test images in the official data. There are 10 different lables in this dataset, such as: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck. The first 36 images is shown above.

The datasets are separated into train( of size 50000), validation(10000), and test datasets(300000) respectively.

In this project, two commonly used CNN models: VGG and ResNet is implemented.

## VGG
Pre-trained VGG16 and VGG19 are included in Keras, here, I build a VGG-like CNN models for object recognition.

### Visualization of VGG model

Here is the screenshot of the output of model.summary().

<p align="center">
<img src="./images/Capturevgg.PNG" alt="Summary of VGG Model Building" style="width:300px;height:300px;" />
</p>

### VGG loss and accuracy versus training epochs
<p align="center">
<img src="./result/vgg_loss.png" alt="Summary of VGG Model Building" style="width:300px;height:300px;" />
</p>

<p align="center">
<img src="./result/vgg_submission.csv" alt="Summary of VGG Model Building" style="width:300px;height:300px;" />
</p>

## ResNet

### ResNet loss and accuracy versus training epochs
The training/validation loss and accuracy versus training epochs are shown below. After 200 epochs, the test accuracy is around 0.90840. But looking carefully, after epoch 75, the training loss is still dropping while testing loss do not get any better since then. So the model seems to overfit.






