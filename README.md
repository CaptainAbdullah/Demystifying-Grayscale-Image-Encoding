# Demystifying Grayscale Image Encoding
Why we need multiple encoding schemes for grayscale images ?

Grayscale images are commonly represented using 8 bits per pixel, which allows for 256 different intensity values. In this representation:
- 0 is typically used to represent black, meaning no intensity.
- 255 is typically used to represent white, indicating maximum intensity.

But sometimes, we have to deviate from standard conventions in order to understand our subject-image effectively.
Some such cases are given below:

`To improve the contrast of images.`
  By encoding black as 255 and white as 0, we can create images with a higher contrast ratio. 
  This can be useful for tasks such as image segmentation and object detection. 

`To make images more compatible with certain file formats.`
  Some image file formats, such as TIFF, allow for multiple grayscale encodings. 
  By encoding images with 255 representing black and 0 representing white, 
  we can make them more compatible with these file formats.
  
`To make images easier to display on certain devices.`
  Some devices, such as older CRT monitors, have limited display capabilities. 
  By encoding images with 255 representing black and 0 representing white, 
  we can make them easier to display on these devices.


# Real World Applications of Inverted Grayscale images
- X-rays: Inverting the grayscale encoding of an X-ray can make it easier to see bone fractures and other abnormalities.
- MRIs: Inverting the grayscale encoding of an MRI can make it easier to see soft tissues, such as the brain and spinal cord.
- CT scans: Inverting the grayscale encoding of a CT scan can make it easier to see blood vessels and other internal structures.
- Ultrasound images: Inverting the grayscale encoding of an ultrasound image can make it easier to see the fetus and other internal structures.

**I took an image of flowers. It was in RGB format. I converted into BGR scheme and then I converted it into grayscale. Then I plot Histogram of the image. The input and output images were:**

## Input Image
<img src="https://github.com/CaptainAbdullah/Demystifying-Grayscale-image-encoding/blob/main/flower.jpg" alt="Input Image">

## Output Image
<img src="https://github.com/CaptainAbdullah/Demystifying-Grayscale-image-encoding/blob/main/output.png" alt="Output Image">

# Key Point: How to understand the encoding scheme!
If the histogram shows that most of the pixel values are close to 0, then the encoding scheme is 0 for black. If the histogram shows that most of the pixel values are close to 255, then the encoding scheme is 255 for black. As we can clearly see that the frequency of 0 is greater than the frequency of 255, hence we can guess that the encoding scheme of the provided image is 0=black and 255=White
