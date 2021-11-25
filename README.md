# CNN_DogVsCat
Created a simple Convolutional Neural Network (CNN) to classify images as either cat or dog

The training set contains 25,000 JPG images of varying dimensions. 
The images are all in color, so they are 3-channel images to account for the standard RGB color scheme.

The dataset used comes from Kaggle. Microsoft is now hosting a copy of the dataset. You can download it here:
https://www.microsoft.com/en-us/download/details.aspx?id=54765
Make sure the dataset is in a folder called Dataset.
Dataset -> PetImages

Things I tweaked to improve accuracy: changed the value of INPUT_SIZE, adding a third convolutional and subsampling layer, 
changed the number of filters, tried using AveragePooling2D subsampling layers instead of MaxPooling2D,
increased the training size, and increased the number of epochs

Results: For the most part, I was only able to achieve a 79% accuracy. 
I did achieve an 85% accuracy when I made the training size 99% (instead of 80%) but I'm not sure if that counts.

The main difference between supervised & unsupervised learning is labeled data. 
This project involves unsupervised learning in that none of the images are explicitly labeled as cat or dog. 
Supervised learning models tend to be more accurate than unsupervised learning models.
With that being said, I'm pretty happy I was able to achieve a similar accuracy (85%) for this project as I was for the predicting diabetes
multilayer perceptron project, which involved supervised learning. It had labeled data and actually told you the outcome 
(whether or not the person developed diabetes). However, this makes me less happy with my accuracy for my MLP diabetes project and makes
me want to tweak that project some more to attain a higher accuracy.
