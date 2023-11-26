# Neural Style Transfer

Neural Style Transfer is a technique leveraging deep neural networks to apply the visual style of one image (the "style image") to the content of another image (the "content image"). This implementation uses TensorFlow and Keras, based on the VGG19 architecture.

## Overview

This project comprises the following components:

1. **Model Architecture:** Utilizes VGG19 for feature extraction, excluding layers for classification and focusing on those capturing style and content information.

2. **Style Transfer:** Transforms a content image with the artistic style of a given style image, producing a stylized image.

3. **Style Adaptation:** Adapts learned style features to new works, preserving original content and artistic integrity.

4. **Evaluation:** Criteria for evaluating style transfer effectiveness include stylistic accuracy, content preservation, and visual appeal.

## Requirements

Ensure the following dependencies are installed:

- Python (>=3.6)
- TensorFlow (>=2.0)
- NumPy
- Matplotlib

Install required packages with:
pip install -r requirements.txt


**Prepare content and style images:**
content_image_path = '/path/to/content/image.jpg'
style_image_path = '/path/to/style/image.jpg'

**For new style**
new_style_image_path = '/content/new_style.png'
(But I am using the same style)

**Optimize the result image for style transfer:** 
1. by increasing the NUM_ITER value from 30 to 1000+
2. By increase the number of epochs to adapt the learned style features to new works in "adapt_style_representation" function.

