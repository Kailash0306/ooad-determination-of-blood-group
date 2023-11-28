# ooad-determination-of-blood-group

# 1.  Import Libraries: 
   - NumPy (`np`): Used for numerical operations.
   - OpenCV (`cv2`): Used for image processing.
   - Matplotlib (`plt`): Used for plotting images.
   - ImageHash (`imagehash`): Used for generating hashes of images.
   - Pillow (`Image` from `PIL`): Used for loading images.

# 2.  Define Pixel Value Mapping Function: 
   - The `pixelVal` function maps intensity levels of pixels to output intensity levels.

# 3.  Vectorize Pixel Value Mapping Function: 
   - `pixelVal_vec` is a vectorized version of the pixelVal function, enabling its application to each value in a NumPy array.

# 4.  Define Image Processing Function (`process_image`): 
   - Reads an image.
   - Converts the image to grayscale.
   - Applies median and Gaussian filters for smoothing.
   - Performs histogram equalization and CLAHE.
   - Applies contrast stretching.
   - Performs edge detection using the Canny edge detector.
   - Saves the processed images with specified prefixes.

# 5.  Main Block for Image Processing (`__main__`): 
   - Provides the paths to two images (`image_path1` and `image_path2`).
   - Calls the `process_image` function for each image with respective output prefixes.

# 6.  Define Image Hashing and Comparison Functions: 
   - `calculate_image_hash`: Converts an image to grayscale and calculates its hash using the dhash algorithm.
   - `compare_images`: Compares the hashes of two images and determines their similarity based on a threshold.

# 7.  Main Block for Image Comparison (`__main__`): 
   - Provides paths to two processed images (`image_path1` and `image_path2`).
   - Sets a similarity threshold.
   - Calls `compare_images` and prints whether the images are similar or not based on the threshold.

