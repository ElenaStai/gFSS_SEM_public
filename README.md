# gFSS_SEM_public

To run the code, three SEM images acquired at different magnifications are required. 
1) The user should begin by opening the script named: gFSS_method.m
2) Within this file, it is necessary to specify two key inputs for each image: the pixel size and the image file name. Under the section labeled “% Pixel size of images”, the user should assign the pixel sizes for the low, middle and high magnification images using the variables ps_first, ps_second, and ps_third, respectively. The input parameters are in red colour.
ps_first = … --> pixel size of low magnification image
ps_second = … --> pixel size for middle magnification image
ps_third = … --> pixel size for high magnification image

Subsequently, under “% Input images”, the corresponding image file names should be entered using the imread function, ensuring that the full file name including the extension (e.g., .tif) is provided. The variables img_first_read, img_second_read, and img_third_read should be used for the low, middle and high magnification images, respectively. 
img_first_read=imread('image_name'); --> low magnification image
img_second_read=imread('image_name'); --> middle magnification image
img_third_read=imread('image_name'); --> high magnification image

3) Output: Upon execution, the code generates a surface image that combines the spatial coverage (measurement range) of the low magnification image with the resolution (pixel size) of the high magnification one.
