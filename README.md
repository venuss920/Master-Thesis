# Thesis
Detection of Windows in Outdoor RGB Images using Camera Behavior Model.


# Research Objectives:
1. Semantic analysis of the windows (Glass).

2. Use a Pre-trained model.

3. Apply State-of-the-Art Deep learning-based models.

4. Examining the mean intersection over union.

5. Semantic analysis - -with two inputs (Numerical + Image) and segmentation as output


# Experimental Setup for Data Acquisition: - https://www.iwt-bodensee.de/mobilitaet/ 

![image](https://github.com/user-attachments/assets/b67d9c0e-5bc1-4632-a4eb-5efd88cac9ca)


   
# Considerations for Object Segmentation:
1. Multi-perspective exposures and data from events [2].

2.  Fusion approach from FGT-NET [5].


3. Fusion while performing Semantic Segmentation (which is Pixel-wise classification).


4. Transfer learning and fine-tuning  for better optimization of results.

 
5. Encoder – Pre-trained model DenseNet201 [6].


6. Decoder – U_net [7].


# Implementation - Feature Fusion (Numerical information with Image Data)
![image](https://github.com/user-attachments/assets/8d71ad1c-bf2d-476c-9bed-923164cd876c)

# Proposed Approach
![image](https://github.com/user-attachments/assets/0bfdffc0-d206-433f-b44e-6d0eb8fe3f3d)



# An instance of Numerical Feature Vector data -
The 12 columns of data are 
(Q = Quality, hdop = Horizontal Degree of 
Precision, ns = nanoseconds, IMU = Inertial Measurement Unit). Note: The table below is an 
example of an image.

![image](https://github.com/user-attachments/assets/2bb1f7ce-66f5-4ebb-a228-c8e755616856)


# Custom Dataset of window glasses. 

1. Images – standard RGB images without depth information of images rather than depth information we would use different numerical data captured from the sensors, the image captured during daytime with the approach; For a better understanding of the complicated scenarios, the image data with event information (Numerical data) in addition to the multi-view perspective of the images would be captured [2]

![image](https://github.com/user-attachments/assets/1f4d58fb-0c82-48bc-928e-231c9539aea3)






# References:

[1] G. Gröger, T. Kolbe, A. Czerwinski, C. Nagel, and P. Henning, “Open GIS city geography markup language (City GML) encoding standard,” Aug. 2008.


[2] L. Yu et al., “Progressive Glass Segmentation,” IEEE Transactions on Image Processing, vol. 31, pp. 2920–2933, 2022, doi: 10.1109/TIP.2022.3162709. 


[3] J. Lin, Y. H. Yeung, and R. W. H. Lau, “Depth-aware Glass Surface Detection with Cross-modal Context Mining,” Jun. 2022. 


[4] H. Mei et al., “Don’t Hit Me! Glass Detection in Real-World Scenes,” in 2020 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), IEEE, Jun. 2020, pp. 3684–3693. doi: 10.1109/CVPR42600.2020.00374.


[5] T. Zhang et al., “A Feature Fusion Method with Guided Training for Classification Tasks,” Comput Intell Neurosci, vol. 2021, pp. 1–11, Apr. 2021, doi: 10.1155/2021/6647220.


[6] G. Huang, Z. Liu, L. van der Maaten, and K. Q. Weinberger, “Densely Connected Convolutional Networks,” Aug. 2016.


[7] O. Ronneberger, P. Fischer, and T. Brox, “U-Net: Convolutional Networks for Biomedical Image Segmentation,” May 2015.

