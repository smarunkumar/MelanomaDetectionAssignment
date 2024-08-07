# CNN model to detect Melanoma
> To build a CNN based multiclass classification model which can accurately detect Melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.

  We are trying to build a multiclass classification CNN model which can accurately detect Melanoma. In addition, model is able to deted following skin diseases.
  
  Actinic keratosis
  Basal cell carcinoma
  Dermatofibroma
  Melanoma
  Nevus
  Pigmented benign keratosis
  Seborrheic keratosis
  Squamous cell carcinoma
  Vascular lesion
  
- What is the business probem that your project is trying to solve?

  Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

- What is the dataset that is being used?

  To build the model we are using dataset consisting of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC).

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Conclusion 1

  Base model with 4 convolutional + 1FC layer, with SGD optimizer without any regularization gave 36% of training accuracy.
- Conclusion 2 

  Base model with 4 convolutional + 1FC layer, with ADAM optimizer without any regularization improved training accuracy with 75% but validation accuracy remained at 50%. But observed faster convergence as compared to SGD optimizer.
- Conclusion 3 

  Created two models with Data augmentation 1) RandomFlip & Random Zoom 2) Random Rotation, Random Contrast and Random Translation. Both the models showed the sign of underfitting with 53-47% training accuracy. The validation accuracy was also around the same range.
- Conclusion 4 

  Due to class imbalance in the data, I used Augmentor to create 500 images for each class. After trying multiple models with different CNN architectures, simple model with with 4 convolutional layers having Maxpooling with dropout, and two fully connected layer gave achieved 86% training accuracy and 80% validation accuracy. However, the model's prediction accuracy on the test dataset was only about 47%. This low accuracy could be attributed to the limited availability of data.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- tensorflow - version 2.17.0
- keras - version 3.4.1
- numpy - version 1.26.4
- Augmentor - version 0.2.12

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was taken as a part of Assignment.

## Contact
Created by [@smarunkumar] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->