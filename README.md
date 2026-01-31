# Lab-05-DIP
1.	Apply mean, median, Gaussian filters.
2.	Apply Laplacian for sharpening.
3.	Implement a 3×3 custom convolution kernel.
4.	Compare noise removal of each filter.
5.	Identify best filter for salt & pepper vs Gaussian noise.
# Code Explanation
This code demonstrates the application of different image smoothing and noise-reduction filters using Python in Google Colab. First, an image is uploaded at runtime, opened using the PIL library, and displayed in its original form. The image is then converted to grayscale and transformed into a NumPy array for processing. A mean filter is applied using convolution with a 3×3 averaging kernel to smooth the image by reducing random noise. Next, a median filter is used to remove salt-and-pepper noise by replacing each pixel with the median value of its neighborhood. After that, a mode filter is implemented using a custom function that replaces each pixel with the most frequently occurring value in its surrounding window, which is useful for preserving edges while reducing noise. A Gaussian filter is also applied, which smooths the image by giving more weight to nearby pixels based on a Gaussian distribution. Finally, all filtered results are displayed together alongside the original grayscale image to visually compare the effects of each filtering technique.
