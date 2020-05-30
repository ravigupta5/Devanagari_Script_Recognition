# Devanagari_Script_Recognition
- Character recognition using fastai PyTorch
- Applying Transfer Learning (ResNet34)

## About Data
- The dataset has been sourced from https://archive.ics.uci.edu/ml/datasets/Devanagari+Handwritten+Character+Dataset.
- This is an image database of Handwritten Devanagari characters
- There are 46 classes (36 alphabets and 10 numerals) of characters with 300 examples each
- Image Format: .png
- Resolution: 32 by 32

![alt text](https://github.com/ravigupta5/Devanagari_Script_Recognition/blob/master/sample_images.PNG?raw=true)

## PART A
- Applyed Transfer Learning
- Used ResNet34 model


## PART B
- Attempted to find best learning rates
- Better accuracy obtained

![alt text](https://github.com/ravigupta5/Devanagari_Script_Recognition/blob/master/learning_rates.PNG?raw=true)

## PART C
- Testing the model
- Used MS Paint to create images with 32x32 size
- Model found to be pretty good in predicting characters 

## PART D
- Model fails when the image size is not 32x32
- Used Python Image Library to resize the input images

![alt text](https://github.com/ravigupta5/Devanagari_Script_Recognition/blob/master/resize_ya.png?raw=true)

**But model can predict only if image backgroud is black and character is white**

![alt text](https://github.com/ravigupta5/Devanagari_Script_Recognition/blob/master/black_white.png?raw=true)

**So the next step to explore could be image processing such that other backgroud images are converted into black blackground with white characters**
