
# Overview
- Image colorization is the process of taking an input grayscale (black and white) image and then producing an output colorized image that represents the semantic colors and tones of the input (for example, an ocean on a clear sunny day must be plausibly “blue” — it can’t be colored “hot pink” by the model).

# The entire (simplified) process can be summarized as:
- Convert all training images from the RGB color space to the Lab color space.
- Use the L channel as the input to the network and train the network to predict the ab channels.
- Combine the input L channel with the predicted ab channels.
- Convert the Lab image back to RGB.
