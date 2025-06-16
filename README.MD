# Image Processing Project

This project contains Python scripts demonstrating various fundamental image processing techniques. 
The goal is to apply and visualize different operations such as color patching, negative imaging, logarithmic transformations, sharpening, noise filtering, and median filtering on sample images.

---

## Contents

- **tf2_engineer.jpg**: Adding a colored patch on a color image  
- **einstein.tif**: Creating a negative image from a grayscale image  
- **pout.tif**: Applying logarithmic and inverse logarithmic transformations  
- **moon.tif**: Sharpening images using spatial and frequency domain unsharp masking  
- **pcb.tif**: Histogram analysis and noise reduction using median and Gaussian filters  
- **pollen.tif**: Applying median filtering on grayscale images  

---

## Requirements

- Python 3.x  
- OpenCV (`cv2`)  
- NumPy  
- Matplotlib  

### Installation

You can install the required libraries using pip:

```bash
pip install opencv-python numpy matplotlib


Usage Instructions
Place all project files (images and scripts) inside the same folder for easier file path management.

You can either use the relative file paths as provided (e.g., "pollen.tif") if your working directory is the project folder, or update the paths according to your system.

Run the Python scripts or Jupyter notebooks in your preferred environment (VSCode, JupyterLab, etc.).

Example code snippet for applying median filter on pollen.tif:

python
Kopyala
Düzenle
import cv2
import matplotlib.pyplot as plt

# Read the grayscale image
img = cv2.imread("pollen.tif", cv2.IMREAD_GRAYSCALE)

# Apply median filter with a 3x3 kernel
filtered_img = cv2.medianBlur(img, 3)

# Display original and filtered images side by side
plt.subplot(1, 2, 1)
plt.imshow(img, cmap='gray')
plt.title("Original Image")
plt.axis('off')

plt.subplot(1, 2, 2)
plt.imshow(filtered_img, cmap='gray')
plt.title("Median Filtered Image")
plt.axis('off')

plt.show()


Project Structure
arduino
Kopyala
Düzenle
image-processing-project/
│
├── tf2_engineer.jpg
├── einstein.tif
├── pout.tif
├── moon.tif
├── pcb.tif
├── pollen.tif
├── Untitled-1.ipynb
└── README.md

Explanation of Techniques Used
Color Patch Addition: Drawing a filled rectangle at the center of a color image using OpenCV.

Negative Imaging: Inverting grayscale pixel intensities to produce a photographic negative effect.

Logarithmic Transformations: Enhancing image contrast by applying log and inverse-log transformations.

Unsharp Masking (Spatial and Frequency Domain): Image sharpening techniques that emphasize edges and details.

Noise Reduction: Applying median filter for salt-and-pepper noise removal and Gaussian blur for smoothing.

Histogram Analysis: Visualizing pixel intensity distribution to understand image characteristics.

Contact
For any questions or issues, please contact:
Abdulsamet ÖZTÜRK
B2180.060066
abdulsametozturk@stu.aydin.edu.tr
