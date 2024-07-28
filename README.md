# Outpainting Image using Stable Diffusion

Demonstrates how to outpaint an image using the `diffusers` library in Python. The task is to extend the given image by adding 128 pixels on each side, ensuring the new pixels blend seamlessly with the original image.

## Prerequisites

- Python 3.7 or higher
- Google Colab (optional for free GPU access)
- Required Python packages:
  - `diffusers`
  - `transformers`
  - `torch`
  - `torchvision`
  - `Pillow`
  - `requests`
  - `matplotlib`
 

 ## Usage 

 Setup Google Colab Environment (Optional):
 
 - Open Google Colab and ensure that GPU is enabled by going to Runtime > Change runtime type and selecting GPU.
 - Download the Image:
 - Download the image from the provided URL.

 ## Explanation

 - The script installs the required libraries diffusers, transformers, torch, and torchvision.
 - It downloads the image from the given Google Drive link using the requests library.
 - The original image is padded by 128 pixels on each side to create a new image with the size 1280x1280.
 - The pre-trained Stable Diffusion model (CompVis/stable-diffusion-v1-4) is loaded using diffusers.
 - The padded image is resized and converted to a tensor for processing by the model.
 - The model generates new pixels to extend the original image naturally, maintaining a seamless transition.
 - The generated image is displayed using matplotlib and saved as outpainted_image.png.

 ## Result

  - The resulting outpainted image will be saved as outpainted_image.png and displayed in the output. The new pixels added should look like a natural extension of the current image.


 ## Installation

 To install the necessary packages, use the following commands:

```bash
pip install diffusers
pip install transformers
pip install torch
pip install torchvision
pip install Pillow
pip install requests
pip install matplotlib
