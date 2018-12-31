# Facial Expression-Recognizer

This notebook contains the code for a facial expression detection algorithm. The data used was acquired from the The [Karolinska Directed Emotional Faces (KDEF)](www.emotionlab.se/kdef/).

KDEF is a dataset of 4900 pictures of human facial expressions of emotion. It was originally developed to be used for psychological and medical research purposes.

The dataset contains 70 individuals (35 male and 35 female), each displaying 7 different emotional expressions, each expression being photographed (twice) from 5 different angles. The expressions are:

    afraid
    angry
    disgusted
    happy
    neutral
    sad
    surprised
    
   <img src="https://github.com/mlsmall/Facial-Expression-Recognition/blob/master/image.jpg" width="477"/>
   
More information on how the data was gathered can be found [here](http://kdef.se/home/aboutKDEF.html).

The architecture used to build this model was ResNet-50, which is a model pre-trained on ImageNet. The initial weights are already trained, so we only have to train the weights in the final layer.

# Model Results and Production

The accuracy achieved was 88.9%. I build a web application for the model. You can try it out yourself here: 

https://facial-exp-recog.herokuapp.com/

Upload a picture a facial expression and it will tell you what it thinks it is, along with how confident it is with that prediction.

One important thing to note about the dataset used is that it was created using young Caucasian men and women. If you try to make a prediction using pictures of older people or people with other skin tones, your results may not be as accurate.

