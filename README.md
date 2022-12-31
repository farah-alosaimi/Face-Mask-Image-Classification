# Face-Mask-Image-Classification-CC-model
 Detect a face mask, using CNN algorithm.  
 Images are processed by using the ImageDataGenerator library to rescale, flipping, shift, and other images process operations. 
 Then, the model can identify whether faces are wearing or not wearing masks based on the processed images that it receives
 
 As a result of training the model with convolutional neural networks to determine whether people wear masks or not, the model's accuracy on the test data is 0.98.
 
# Discovering Directory and Paths
After declaring the paths of the dataset,the directory contains three main folders already divided into three chunks to train, test, and validate, each of which contains two directory "withmask" or "withoutmask". Dataset -train -Withmask -Withoutmask -test -Withmask -Withoutmask -validation -Withmask -Withoutmask The dataset contains 11792 pictures and labels. Using the "OS" library, I found out how many images have masks and how many don't.
