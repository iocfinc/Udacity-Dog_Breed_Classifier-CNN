# Udacity-Dog_Breed_Classifier-CNN

## Background

This project was created as part of the requirements for Udacity's Deep Learning Nanodegree. This is the project for the Convolutional Neural Network module of the course.

This was done with the use of transfer learning making use of the InceptionV3 bottleneck features. The inceptionV3 model was used as a fixed feature extractor and I added a classifier network near the end to match the number of dog breeds expected. The model was able to meet the objective of training the model with at least 60% accuracy. The test accuracy received by the model was at 81.5789%.

Additionally, there was an added logic to the project where a dog or face detector has been added to check for the presence of a dog or human face in the image. The resulting final model is able to check for the presence of a dog or human (or a human that looks like a dog) and provide the closest dog breed of the detected dog/human. It is also tested to have some error handling in cases where no dog or human face is detected on the image.

## Results

The model was tested on images downloaded from the internet and the results are in the `dog_app.ipynb` but a screen shot of the results is also seen below.

<p align="center"><img src='.\screenshot\2019-01-16 04_26_41-dog_app.png' width=500px alt = "boxer"></p>

<p align="center"><img src='.\screenshot\2019-01-16 04_27_09-dog_app.png' width=500px alt = "boxer"></p>

<p align="center"><img src='.\screenshot\2019-01-16 04_26_58-dog_app.png' width=500px alt = "boxer"></p>

<p align="center"><img src='.\screenshot\2019-01-16 04_27_17-dog_app.png' width=500px alt = "boxer"></p>

## Possible Improvements

A possible improvement on the model would be the use of the bottleneck features and finetuning the pre-trained model to achieve higher accuracy. This would involve updating all the parameters of the model again to fit our dataset but from what I saw in the PyTorch documentations and in the PyTorch scholarship slack channel the results for finetuning tended to be better.