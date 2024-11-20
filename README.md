# Image Processing with Fourier Transforms

This repository demonstrates various image processing techniques using Fourier Transforms (FT) to manipulate and analyze images. The code applies both 1D and 2D Fourier Transforms to perform operations such as frequency analysis, convolution, and spatial transformations.

## Key Features

### 1. **Image Loading and Display**
   - The code reads an image (`t1.jpg`) and displays both the original image and a specific slice (the first color channel).

### 2. **Frequency Domain Analysis**
   - The Discrete Fourier Transform (DFT) is applied to a specific row (128th row) of the image to compute and visualize both the magnitude and phase.
   - The 2D Fourier Transform of the entire image is computed, and its magnitude is visualized using a logarithmic scale for better clarity.
   - The zero-frequency components are centered using `fftshift`, and the shifted frequency spectrum is displayed alongside the original image.

### 3. **Image Convolution in the Frequency Domain**
   - Convolution is performed between two images (a circular mask and an arbitrary image) in the frequency domain by multiplying their Fourier Transforms. The result is then transformed back to the spatial domain using the inverse Fourier Transform (`ifft2`).
   - The convolved image is displayed alongside the original images for comparison.

### 4. **Zooming in on the Frequency Spectrum**
   - The Fourier Transform of a CT image is computed and zoomed into a specific region of its frequency spectrum.
   - The zoomed-in frequency spectrum is then inverse transformed back into the spatial domain, demonstrating how different frequency regions affect the image.

### 5. **Shifting and Rotating Images in the Frequency Domain**
   - The code demonstrates how to shift an image in the frequency domain by applying a phase shift. The resulting shifted image is visualized alongside the original.
   - Image rotation is also performed in both the spatial and frequency domains to observe the effects on the image’s appearance.

