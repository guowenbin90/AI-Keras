## Code examples
https://keras.io/examples/
- Computer Vision
- Natural Language Processing
- Structured Data
- Timeseries
- Audio Data
- Generative Deep Learning
- Reinforcement Learning
- Graph Data
- Quick Keras Recipes

## Keras Applications
https://keras.io/api/applications/  
Keras Applications are deep learning models that are made available alongside pre-trained weights. These models can be used for prediction, feature extraction, and fine-tuning.

[**What Is The Input Shape In A Keras Layer?**](https://wandb.ai/ayush-thakur/dl-question-bank/reports/Keras-Layer-Input-Explanation-With-Code-Samples--VmlldzoyMDIzMDU#:~:text=4%20%3D%2048%20elements.-,What%20Is%20The%20Input%20Shape%20In%20A%20Keras%20Layer%3F,(layers)%20is%20computed%20automatically.)

In a Keras layer, the input shape is generally the shape of the input data provided to the Keras model while training. The model cannot know the shape of the training data. The shape of other tensors(layers) is computed automatically.  
Each type of Keras layer requires the input with a certain number of dimensions:
- **Dense layers** require inputs as `(batch_size, input_size)`
- **2D convolutional layers** need inputs as:
  - if using channels_last: `(batch_size, imageside1, imageside2, channels)`
  - if using channels_first: `(batch_size, channels, imageside1, imageside2)`
- **1D convolutions and recurrent layers** use `(batch_size, sequence_length, features)`
- **The shape of other tensors** is computed based on the number of units provided along with other particularities like `kernel_size` in the `Conv2D` layer.


