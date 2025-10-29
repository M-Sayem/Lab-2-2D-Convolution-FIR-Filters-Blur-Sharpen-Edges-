# Lab 2: 2D Convolution & FIR Filters (Blur, Sharpen, Edges)

This MATLAB lab explores spatial filtering of images using 2D convolution and FIR filter kernels.  
It demonstrates how low-pass, high-pass, and edge-detection filters affect image features.

## Sections

1. **Impulse Response:** Visualizes the effect of a 3×3 average filter using a delta image.
2. **Low-Pass Filtering:** Compares box filters of different sizes and a Gaussian filter; highlights that Gaussian provides smoother results and better frequency characteristics.
3. **Unsharp Masking (Sharpening):** Combines the original image with a high-frequency mask to enhance details.
4. **Edge Detection:** Applies Sobel filters (horizontal and vertical gradients) and a Laplacian operator to highlight edges.
5. **Correlation vs Convolution:** Demonstrates the kernel-flip difference and verifies numerical equivalence between `conv2` and `imfilter`.
6. **Boundary Handling:** Compares how replicate, symmetric, and circular padding affect image borders.
7. **Reflections:**
   - Gaussian is preferred over a large box filter because it avoids abrupt cutoffs and reduces ringing.
   - Separability (two 1D filters instead of one 2D) significantly reduces computational cost.
   - Boundary modes alter how edges and corners are treated in filtered images.
