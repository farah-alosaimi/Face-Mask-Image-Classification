# Face-Mask-Image-Classification-CNN-model
 Detect a face mask, using CNN algorithm.  
 Images are processed by using the ImageDataGenerator library to rescale, flipping, shift, and other images process operations. 
 Then, the model can identify whether faces are wearing or not wearing masks based on the processed images that it receives
 
 As a result of training the model with convolutional neural networks to determine whether people wear masks or not, the model's accuracy on the test data is 0.98.
 
# Discovering Directory and Paths
After declaring the paths of the dataset,the directory contains three main folders already divided into three chunks to train, test, and validate, each of which contains two directory "withmask" or "withoutmask". Dataset -train -Withmask -Withoutmask -test -Withmask -Withoutmask -validation -Withmask -Withoutmask The dataset contains 11792 pictures and labels. Using the "OS" library, I found out how many images have masks and how many don't.

# Plotting Images
To plot the images, i used the imread() function from CV library.

<img width="455" alt="image" src="https://user-images.githubusercontent.com/87046282/210136673-ac122fb9-4ca6-46fd-a225-b2a7d723fcd0.png">

# Image Processing
The image processing phase now starts, using the ImageDataGenerator library. With the ImageDataGenerator() function we can rescale-multiply- the data by 1/255 ,rotate the pictures by 40 degrees ,shift the height and width by 0.2 , shear intensity is 0.2 , zoom ranges is 0.2, and randomly flip the pictures.

<img width="254" alt="image" src="https://user-images.githubusercontent.com/87046282/210136736-3d594150-5902-4225-87cc-8041a0cc6c8f.png">


After applying image processing to all the images, executed by the flow_from_directory() function, which takes the path to a directory & generates augmented data. This function will resize the images to 95 x 95, batch size is set to 15, colour mode of the images goes to RGB, which means the pictures stay colourful, class mode is categorical, and we need to shuffle the data in order to avoid pattern cheating.

<img width="367" alt="image" src="https://user-images.githubusercontent.com/87046282/210136800-5df056c5-52c3-4025-ba15-8893156b0592.png">



# The model
The structure of the convolutional neural network model

<img width="450" alt="image" src="https://user-images.githubusercontent.com/87046282/210136862-e5c3489a-1502-41bf-9741-4f1eac0050bf.png">

# Train & Test

<img width="417" alt="image" src="https://user-images.githubusercontent.com/87046282/210136887-f0e1832e-d089-465d-9bf5-ef87b7cc679d.png">


# Evalution
classification report showing the main classification metrics/ accuracy .. ect

<img width="401" alt="image" src="https://user-images.githubusercontent.com/87046282/210136910-f162a97d-4ba7-49a0-893d-8ff3e81080b5.png">


