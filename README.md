[Veiw Project White Paper PDF](https://github.com/deep-model/Computer_Vision_with_Canny-Edge_Detection/blob/main/Final_Project_Report-M.Harper.pdf)

# Multistage Edge Detection with Canny Algorithms 
<p align="left">
  
<img width="600" height="400" alt="image" src="https://github.com/deep-model/Computer_Vision_with_Canny-Edge_Detection/blob/main/street_picture_2.jpg" />
<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/221e54cb-a21b-4a33-894f-1c262b42a39e" />

</p>

## Computer Vision and Image Processing 
Matthew Harper 

Image features in image processing represent essential visual and mathematical characteristics that 
convey meaningful information within an image. These features include observable attributes such 
as shape, color, texture, lines, and edges, as well as mathematical descriptors such as pixel 
intensity, gradients, slope, angle or direction, magnitude, noise, and frequency [1, 2]. Moreover, 
feature selection and detection is a fundamental concept in image processing and computer vision, 
enabling the identification of prominent and distinctive patterns while reducing complex pixel
level data into structured and analyzable components [1, 2]. 

In addition, edge detection is a critical image segmentation and feature detection technique which 
focuses on identifying object boundaries through abrupt changes in image intensity, commonly 
modeled using step, ramp, and roof-edge intensity profiles [2, 4]. However, when comparing the 
available edge detection approaches, the multistage Canny edge detection algorithm remains one 
of the most widely used due to its robust and optimal performance of its multistage image 
segmentation algorithm.  

The Canny method was specifically designed to satisfy three primary objectives which include 
achieving a low error rate with minimal noise response, detection of accurate edge localization, 
and obtaining a prominent true edge [2, 4]. These objectives are approximated mathematically 
through the use of Gaussian smoothing to reduce noise, gradient magnitude and direction 
computation to detect candidate edges, non-maximum suppression to refine edge thickness, and 
thresholding with edge linking to preserve meaningful edges while suppressing false detections [2, 
4]. 

The reliable and well-localized edges produced by the Canny edge detection algorithm provide a 
strong foundation for subsequent image processing tasks, particularly image segmentation. Image 
segmentation relies on dividing an image into meaningful regions based on similarity or 
discontinuity in intensity,  and Canny-based edge characteristics are especially effective for 
segmentation approaches that depend on gradient intensity, magnitude, and direction [2, 4]. As a 
result, Canny edge detection is an important technique in image segmentation, object recognition, 
and many computer vision applications [1–4]. 

# The Multistage Canny Edge Detector  
Edge detection can be defined as a method utilized for the segmentation of an image(s) based on 
the identification of rapid and abrupt changes in intensity, referred to as local minima and local 
maxima in the gradient. 
Moreover, edge detection models can also be classified based on their intensity profiles or the way 
in which the edge transitions in intensity. The step-edge or ideal edge is an edge characterized as 
having two distinct binary intensities occurring over one pixel. The figure below illustrates this 
step edge phenomenon. Images with intensity profiles described as having slowly increasing slope 
inversely proportionate to the degree to which the edge is blurred is known as a ramp profile. 
Roof-edge is another commonly observed image edge detection intensity profile in which a model 
of lines through a localized region are observed cresting to a point [1, 2, 4].  
