# Motivation
Going through object detection (using Convolutional neural network (CNN)) branch in artifical intligince (AI) was a blast :boom: for me.

Seeing how every step in processing the image gives a bit of knwolage on the big picture with many and many bits getting together at the end to give a final descion from the input was fascinating.

All that was great but needed much computer power and memory to save and proccess the data through the CNN network.
# About
We tried to take the concept of the famous (ResNet) and apply it in a shallow network with some modifications on it.

# Result
We compared against a base model on github by Irtaza which can be found [here](https://github.com/Irtza/Keras_model_compression)

The networks below were both trained using [Kaggle Cats and dogs dataset](https://www.microsoft.com/en-us/download/details.aspx?id=54765)

| Model | Final | Base |
|-------|:-----:|------|
| Parameters | 35,458 | 18,893,570 |
| Train time (Per epoch)(s) | 80 | 240 |
| Train accuracy (%) | 0.90 | 0.98 |
| Test accuracy (%) | 0.70 | 0.76 |
| Memory footprint (Mb) | 0.13 | 72 |

# Steps
We started from the base model that was linked above and then move to test and try other approaches :

### Double the layers:
We first tried to only double the amount of layers that we have and narrow the network down, this gave some pleasing results and we started to undetrstand more of what is happening. You can find the notebook for it [here](https://github.com/Saria-houloubi/CNN_keras_model_compression/blob/master/Base%20model-doubled%20layers.ipynb)

### Exploring more models :eyes:
As we kept on changing some parameters in the aim to get something better, but all the results were not much  pleasing :sob:, so we went on reading and searching through the great networks that are out there.

**ResNet:** was the network that caught my eye because it was easy to understand and implement anywhere. So we started digging deeper in it which lead to implementing **ResNet50** which can be found [here](https://github.com/Saria-houloubi/CNN_keras_model_compression/blob/master/ResNet.ipynb)

Now we are in this huge network with some huge parameters count :dizzy_face:!.

### Combine the ideas
While reading all about ResNet and how great it proformed in many places I wanted to try the same approache, but in a shallower network.

So after a bit of tuning things around we got our network to implement the ResNet blocks in it, which can be found[here](https://github.com/Saria-houloubi/CNN_keras_model_compression/blob/master/Base%20model%20using%20ResNet.ipynb).

### Some extras :art:
Until here we got some great results so we saved it first :smiley:, then tried some change in parameters, layer order and type.
Which ended up in our final structure [here](https://github.com/Saria-houloubi/CNN_keras_model_compression/blob/master/Base%20model%20final%20structure.ipynb)

### Final Notes
This was my graduation project to get my degree in Computer Enginnering :computer: at Tishreen university, I have not uploaded the paper work (Writen in Arabic mostly) here but if anyone needs them would be glad to share.
 
 
 Made with :heart:
