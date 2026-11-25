# Exp3-Sobel-edge-detection-filter-using-CUDA-to-enhance-the-performance-of-image-processing-tasks.
<h3>AIM:</h3>
<h3>ENTER YOUR NAME</h3>
<h3>ENTER YOUR REGISTER NO</h3>
<h3>EX. NO</h3>
<h3>DATE</h3>
<h1> <align=center> Sobel edge detection filter using CUDA </h3>
  Implement Sobel edge detection filtern using GPU.</h3>
Experiment Details:
  
## AIM:
  The Sobel operator is a popular edge detection method that computes the gradient of the image intensity at each pixel. It uses convolution with two kernels to determine the gradient in both the x and y directions. This lab focuses on utilizing CUDA to parallelize the Sobel filter implementation for efficient processing of images.

Code Overview: You will work with the provided CUDA implementation of the Sobel edge detection filter. The code reads an input image, applies the Sobel filter in parallel on the GPU, and writes the result to an output image.
## EQUIPMENTS REQUIRED:
Hardware – PCs with NVIDIA GPU & CUDA NVCC
Google Colab with NVCC Compiler
CUDA Toolkit and OpenCV installed.
A sample image for testing.

## PROCEDURE:
Tasks: 
a. Modify the Kernel:

Update the kernel to handle color images by converting them to grayscale before applying the Sobel filter.
Implement boundary checks to avoid reading out of bounds for pixels on the image edges.

b. Performance Analysis:

Measure the performance (execution time) of the Sobel filter with different image sizes (e.g., 256x256, 512x512, 1024x1024).
Analyze how the block size (e.g., 8x8, 16x16, 32x32) affects the execution time and output quality.

c. Comparison:

Compare the output of your CUDA Sobel filter with a CPU-based Sobel filter implemented using OpenCV.
Discuss the differences in execution time and output quality.

## PROGRAM:
TYPE YOUR CODE HERE

## OUTPUT:
SHOW YOUR OUTPUT HERE

## RESULT:
Thus, the program has been executed successfully using CUDA to perform Sobel edge detection on an image using GPU parallel processing.
Answers to the Questions

1. What challenges did you face while implementing the Sobel filter for color images?
- Handling RGB channels separately was challenging.
- Converting the color image into grayscale was necessary.
- Managing pixel boundaries and memory allocation was difficult.
2. How did changing the block size influence the performance of your CUDA implementation?
- Smaller block sizes may increase execution overhead.
- Larger block sizes can improve parallel processing.
- The best block size depends on GPU resources and image size.
3. What were the differences in output between the CUDA and CPU implementations? Discuss any discrepancies.
- Both implementations produced similar edge-detection results.
- CUDA executed faster due to parallel processing.
- Minor differences may occur due to rounding and pixel calculations.
4. Suggest potential optimizations for improving the performance of the Sobel filter.
- Use shared memory to reduce global memory access.
- Optimize CUDA block and grid dimensions.
- Reduce unnecessary memory transfers.
- Process multiple pixels in parallel.

### Tools Required:
1. NVIDIA CUDA Toolkit
2. NVIDIA GPU
3. Google Colab
4. C/C++ compiler (NVCC)
5. OpenCV library
6. Python and Matplotlib
