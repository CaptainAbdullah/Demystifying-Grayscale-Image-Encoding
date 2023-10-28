# Demystifying Grayscale image encoding
Why we need multiple encoding schemes for grayscale images ?

Grayscale images are commonly represented using 8 bits per pixel, which allows for 256 different intensity values. In this representation:
<li>0 is typically used to represent black, meaning no intensity.</li>
<li>255 is typically used to represent white, indicating maximum intensity.</li>
<br>
But sometimes, we have to deviate from standard conventions in order to understand our subject-image effectively.
Some such cases are given below:<br>
<b>To improve the contrast of images.</b>
  By encoding black as 255 and white as 0, we can create images with a higher contrast ratio. 
  This can be useful for tasks such as image segmentation and object detection. 

<b>To make images more compatible with certain file formats.</b> 
  Some image file formats, such as TIFF, allow for multiple grayscale encodings. 
  By encoding images with 255 representing black and 0 representing white, 
  we can make them more compatible with these file formats.
  
<b>To make images easier to display on certain devices.</b> 
  Some devices, such as older CRT monitors, have limited display capabilities. 
  By encoding images with 255 representing black and 0 representing white, 
  we can make them easier to display on these devices.

<h3>Real World Applications of Inverted Grayscale images</h3>
<li>X-rays: Inverting the grayscale encoding of an X-ray can make it easier to see bone fractures and other abnormalities.</li>
<li>MRIs: Inverting the grayscale encoding of an MRI can make it easier to see soft tissues, such as the brain and spinal cord.</li>
<li>CT scans: Inverting the grayscale encoding of a CT scan can make it easier to see blood vessels and other internal structures.</li>
<li>Ultrasound images: Inverting the grayscale encoding of an ultrasound image can make it easier to see the fetus and other internal structures.</li>
