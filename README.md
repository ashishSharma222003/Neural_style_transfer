# Neural_style_transfer


To set up and run the notebook containing this code snippet, you'll need the following dependencies:

1.TensorFlow: You can install TensorFlow using pip install tensorflow.

2.NumPy: Install NumPy with pip install numpy.

3.Matplotlib: Install Matplotlib with pip install matplotlib.

4.Scipy: Install Scipy with pip install scipy.

5.PIL (Python Imaging Library): Install PIL with pip install pillow.


You'll also need the two image files, one for the content image and another for the style image. Make sure to provide the file names in the code where specified.

Here's a summary of the code snippet:

-It starts by importing the necessary packages and libraries.

-VGG-19, pretrained on the ImageNet dataset, is loaded using tf.keras.applications.VGG19.

-The layers of VGG-19 are printed to check the names.

-Content cost function, style cost function, style layers, and total cost function are defined.

-The content image and style image are loaded and reshaped into tensors.

-The generated image is initialized, and noise is added to it.

-The VGG-19 model is loaded again using the defined layer outputs.

-The content and style targets are computed.

-Functions for clipping values and converting tensors to images are defined.

-The training step is defined, which computes the style and content costs, updates the generated image using gradient descent, and clips its values.

-The model is trained for a specified number of epochs, and the generated image is saved at intervals.

-Finally, the content image, style image, and generated image are displayed.
