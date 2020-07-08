[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

In this project, I learnt how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, my algorithm identifies an estimate of the dog’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

Along with exploring state-of-the-art CNN models for classification and localization, I made important design decisions about the user experience for your app. In this project I used both my own CNN model coded from scratch an I also used the transferred learning model from 

These are the architectures of each model:
**The one I built from scratch**

```

Net(
  (conv1): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
  (bn1): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
  (conv2): Conv2d(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
  (bn2): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
  (conv3): Conv2d(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
  (bn3): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
  (conv4): Conv2d(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
  (bn4): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
  (conv5): Conv2d(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
  (bn5): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
  (fc1): Linear(in_features=32768, out_features=1024, bias=True)
  (fc2): Linear(in_features=1024, out_features=512, bias=True)
  (fc3): Linear(in_features=512, out_features=133, bias=True)
  (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
  (dropout): Dropout(p=0.5)
)
```
**The one I built from scratch**


### Instructions

The important parts of this project are in the `dog_app.ipynb` file. However, if you wish to follow this project and run it locally, you can follow [these instructions](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/tree/master/Bike%20Sharing%20Patterns%20Neural%20Network%20for%20Nanodegree#instructions) but changing the command of Step 1 to `https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/tree/master/CNN%20Dog%20Breed%20Classifier`. 





