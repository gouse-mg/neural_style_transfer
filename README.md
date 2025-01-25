# nueral_style_transfer
paper_implementation01
# Neural Style Transfer: Low-Level Implementation

This repository contains a low-level implementation of neural style transfer using TensorFlow and the VGG19 pretrained model. The aim is to combine the content of one image with the style of another to produce a new, stylized image.

## Key Features
- **Content Extraction:** Extracts the features of the content image using the VGG19 model.
- **Style Representation:** Computes the Gram matrix of the style layers to capture texture information.
- **Loss Functions:** Implements content loss and style loss to guide the optimization process.
- **Optimization:** Uses TensorFlow's GradientTape and Adam optimizer for iterative canvas updates.

## Requirements
- Python 3.7 or higher
- TensorFlow 2.x
- NumPy
- Pillow
- Matplotlib

# doubt
-why do we need the content loss if we can initialize the canvas with the content image? To avoid a circumstance where the model entirely ignores the content features, we could set the learning rate low so that the basic features and some high-level features remain intact. Any insights or clarifications from the community would be greatly appreciated!


