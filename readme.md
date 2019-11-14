Name : Prakash Shanmugam
Email : careers.prakash@gmail.com

Convolution : Convolution is a layer to extract features from an input image. Convolution preserves the relationship between pixels by preserving image features using small squares of input data. It is a mathematical operation that takes two inputs such as image matrix and a filter or kernel.

Filters/Kernels : Filters are technique for modifying or enhancing an image. One can filter an image to emphasize certain features or remove other features. Image processing operations implemented with filtering include smoothing, sharpening, and edge enhancement.

Epochs : Epochs is a hyperparameter that defines the number times that the learning algorithm will work through the entire training dataset. One epoch means that each sample in the training dataset has had an opportunity to update the internal model parameters. An epoch is comprised of one or more batches. The number of epochs is traditionally large, often hundreds or thousands, allowing the learning algorithm to run until the error from the model has been sufficiently minimized.
Example: Let's say we have 1000 samples of data with a batch size of 10 and we want to run 3 epochs. In each epoch, we have (1000/10 = 100 batches or iterations). Each batch passes through our model, so we have 100 iterations/epoch, as we have 3 epochs which is equal to 3*100=300 iterations for training.


1x1 convolution : 1×1 Convolution is a orchestration layer of the network, whose main purpose is dimensionality reduction (either increase or decrease of dimensions). Its main purpose is to collapse all input pixel channels into one output pixel. For example, if you have a 28×28 image with 32 channels for each input pixel and if you apply a 10 1×1 kernels then it would collapse all 32 channels into just 10 channels of each pixel.

| 28×28, 32 |  --> | 10, 1×1|  --> | 28×28, 10|


3x3 convolution : 3x3 Convolution is an important type of convolution as it is used for detecting edge, textures, patterns, parts and objects.


Feature map : The feature map is the output of one filter applied to the previous layer. A given filter is drawn across the entire previous layer, moved one pixel at a time. Each position results in an activation of the neuron and the output is collected in the feature map. You can see that if the receptive field is moved one pixel from activation to activation, then the field will overlap with the previous activation by (field width - 1) input values.

Activation function : Activation function decides, whether a neuron should be activated or not by calculating weighted sum and further adding bias with it. The purpose of the activation function is to introduce non-linearity into the output of a neuron.

Receptive field : The receptive field can be briefly defined as the region in the input space that a particular CNN’s feature is looking at .A receptive field of a feature can be described by its center location and its size.However, not all pixels in a receptive field is equally important to its corresponding CNN’s feature.Within a receptive field, the closer a pixel to the center of the field, the more it contributes to the calculation of the output feature. Which means that a feature does not only look at a particular region in the input image, but also focus exponentially more to the middle of that region.
