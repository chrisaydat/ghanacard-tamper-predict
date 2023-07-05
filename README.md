# ghanacard-tamper-predict
# Ghana/Ecowas Card Image Tampering Detection
# Chris Aydat (Chris F.O Ayeh-Datey)

This Python script is designed to detect tampering in images using the Structural Similarity Index (SSIM) and image processing techniques. It compares an original image with a potentially tampered image and highlights the differences.

## Dependencies

The following dependencies are required to run the script:
- `scikit-image` (imported as `skimage`)
- `opencv-python` (imported as `cv2`)
- `imutils`
- `requests`
- `PIL` (imported as `Image`)

You can install the required dependencies using the following command:

```shell
pip install scikit-image opencv-python imutils requests pillow
```

## Usage

1. Clone or download the repository to your local machine.

2. Run the `image_tampering_detection.py` script using Python.

3. The script will perform the following steps:

   - Create necessary directories to store the images.
   - Fetch the original and tampered images from the provided URLs.
   - Print the format and size information of both images.
   - Resize the images to the same size (400x400 pixels) for comparison.
   - Save the resized images in the `ghscard_tamper/images` directory.
   - Display the original and tampered images.
   - Load the images using OpenCV and convert them to grayscale.
   - Compute the Structural Similarity Index (SSIM) between the images.
   - Calculate the difference image and display the SSIM score.
   - Apply a threshold to the difference image and find contours.
   - Draw rectangles around the detected contours on the original and tampered images.
   - Display the original image with contours.
   - Display the tampered image with contours.
   - Display the difference image.
   - Display the thresholded image.

4. Examine the displayed images to identify any tampering. Contours indicate areas of significant difference between the original and tampered images.

Note: The script uses specific URLs for the original and tampered images as examples. You can modify the URLs to use your own images by replacing the URL strings in the code.

## License

This script is released under the [MIT License](LICENSE).

Feel free to contribute and provide feedback!
