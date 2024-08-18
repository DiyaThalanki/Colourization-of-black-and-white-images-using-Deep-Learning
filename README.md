# Colorization of Black and White Images using Deep Learning

This project uses a deep learning model to colorize black and white images. The process involves converting RGB images to LAB format, predicting the A and B channels using a pre-trained model, and then converting the LAB image back to RGB format to produce the final colorized image.

## Concept Explanation

1. **Convert RGB to LAB:** RGB images are converted to LAB images. LAB stands for Lightness (L), A (green-red color component), and B (blue-yellow color component).
2. **Extract L Channel:** The L channel (lightness) is extracted from the LAB image.
3. **Predict A and B Channels:** The L channel is fed into a deep learning model to predict the A and B channels.
4. **Combine Channels:** The predicted A and B channels are combined with the L channel to form the LAB image.
5. **Convert LAB to RGB:** The LAB image is then converted back to RGB format, giving the final colorized output.

## Prerequisites

To run this project, you need to have the following installed:

- Python 3.x
- OpenCV
- NumPy

You also need to download the pre-trained models used in this project. The required files are:

- `colorization_deploy_v2.prototxt`
- `pts_in_hull.npy`
- `colorization_release_v2.caffemodel`

These files should be placed in the `models/` directory.
