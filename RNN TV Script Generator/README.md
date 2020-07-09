# Project Overview

In this project I have developer a Recurrent Neural Network with Long Short Term Memory neurons (LSTM) which main purpose is to be trained in the plot of the chapters of the Seinfeld TV Show and produce as an output a new generated script that could act as a new chapter of the show. 

In the project I have used some data preprocessing methods such as tokenization, creating a vocabulary, batching and so on. For more details about all the methods implemented [check the notebook](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/blob/master/RNN%20TV%20Script%20Generator/dlnd_tv_script_generation.ipynb)

The neural network used consists of a RNN with an embedding layer, 3 LSTM layers and a final linear layer. The loss function used was a Cross Entropy Loss and the optimizer chosen was Adam. For more details about how this model is implemented, again, [check the notebook](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/blob/master/RNN%20TV%20Script%20Generator/dlnd_tv_script_generation.ipynb).
These are just some of the hyper-paramters used in the model and during the training, below them you can find the justification of some of their choice: 
- Dropout : 20%
- Embedding dimensions : 200
- Hidden dimensions : 256
- Sequence length : 8
- Epochs : 10
- Batch size : 128
- Learning Rate : 0.001
---
- **Sequence length:** considering that the average amount of words per line is 5 and that this amount will probably be influenced to the low side by sentences of short replies (like yes/no/maybe) I decided that 8 would be a good number for the sequence lenght for predicting the next target word (considering the information of a line length of words).
- **Batch size:** after testing with batch sizes of 32 and 64 I realised that this network could easily handle in terms of computational time a higher number so I went for 128.
- **Number of epochs:** I considered 10 epochs good enough for this experimental/learning exercise as they are enough for giving me insight on how good the hyper-paramter tunning and network went and not too long for making training too long. I reckon the network was still learning and with some more epochs (maybe between 30-50) the training could have still improved (maybe to get close to 3).
- **Learning rate:** 0.001 seemed a sensible value considering that the dropout on the final layer acts as regularization letting me have higher learning rate. 0.01 also gives good results but the improved is not as smooth as with 0.001.
- **Embedding dimensions:** 200 are good enough for the network to learn semantics and learn more without costing too much computationally.
- **Hidden dimensions:** 256 is a good number of networks keeping a good efficency although I believe in this case 512 despite taking longer for training would not overfit as I believe my results still gave quite some room for improvement.
- **Number of layers:** from the lesson previously mentioned I took that 3 layers is usually better than 2 unless it overfits and in this case as I tested it did not overfit using 3 layers.
- **Dropout 20%:** It added some regularization to the network and prevented overfitting.
---

## Outcome

This model and set up returned a training error of 3.6. This is a part of the TV script it generated, for the full script [check the generated text file](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/blob/master/RNN%20TV%20Script%20Generator/generated_script_1.txt).

```
george: what?

kramer: no, no. no, no, no, no, i can't be able to get the call on the car.

george: well, i don't even think it's going to be.

kramer: oh, yeah. i don't know what i was thinking, and i think i could get it.

kramer: well, i think i could do this, but you know what?

kramer: i can't believe this would get a little problem.

jerry:(to the cashier, still) i think it's a good mistake.

george:(pointing at his forehead) hey, jerry, i don't want to see you.

jerry:(to jerry) oh, you know, i can't.

jerry: oh, that's right! it's not gonna get a little problem.

george: well, i guess it's going to have a good problem.

jerry: what do you mean?

```

### Instructions

The important parts of this project are in the `dlnd_tv_script_generation.ipynb` file. However, if you wish to follow this project and run it locally, you can follow [these instructions](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/tree/master/Bike%20Sharing%20Patterns%20Neural%20Network%20for%20Nanodegree#instructions) but changing the command of Step 1 to `https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/new/master/RNN%20TV%20Script%20Generator`.
### License

MIT License

Copyright (c) 2020 Mateo Randulfe
