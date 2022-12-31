# Face-Mask-Image-Classification-CC-model
 Detect a face mask, using CNN algorithm.  
 Images are processed by using the ImageDataGenerator library to rescale, flipping, shift, and other images process operations. 
 Then, the model can identify whether faces are wearing or not wearing masks based on the processed images that it receives
 
 As a result of training the model with convolutional neural networks to determine whether people wear masks or not, the model's accuracy on the test data is 0.98.
 
# Discovering Directory and Paths
After declaring the paths of the dataset,the directory contains three main folders already divided into three chunks to train, test, and validate, each of which contains two directory "withmask" or "withoutmask". Dataset -train -Withmask -Withoutmask -test -Withmask -Withoutmask -validation -Withmask -Withoutmask The dataset contains 11792 pictures and labels. Using the "OS" library, I found out how many images have masks and how many don't.

# Image Processing
The image processing phase now starts, using the ImageDataGenerator library. With the ImageDataGenerator() function we can rescale-multiply- the data by 1/255 ,rotate the pictures by 40 degrees ,shift the height and width by 0.2 , shear intensity is 0.2 , zoom ranges is 0.2, and randomly flip the pictures.

![alt text](http://url/to/img.png)

After applying image processing to all the images, executed by the flow_from_directory() function, which takes the path to a directory & generates augmented data. This function will resize the images to 95 x 95, batch size is set to 15, colour mode of the images goes to RGB, which means the pictures stay colourful, class mode is categorical, and we need to shuffle the data in order to avoid pattern cheating.

image
