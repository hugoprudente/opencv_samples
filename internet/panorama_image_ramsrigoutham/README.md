# Panorama Image by Ramsri Goutham

The code  snippet shown below is for simple image stitching of two images in OpenCV . It can easily be modified to stitch multiple images together and create a Panorama.

OpenCV also has a stitching module which helps in achieving this task and which is more robust than this.  The code presented here will help in understanding the major steps involved in image stitching algorithm. 

## Theory

The main parts of stitching algorithm are
 - Finding Surf descriptors in both images
 - Matching the surf descriptors between two images
 - Using  RANSAC to estimate the homography matrix using the matched surf descriptors.
 - Warping the images based on the homography matrix.

## What was fixed?

This code is originally coded for OpenCV 2.4.x, and now is fixed to work with OpenCV 3.1.x

## Explanation

## How to use?

```sh
$ ./Panorama <img1> <img2>
```
## Input

![Image 1](https://ramsrigoutham.files.wordpress.com/2012/11/panorama_image1.jpg?w=300&h=225)
![Image 2](https://ramsrigoutham.files.wordpress.com/2012/11/panorama_image2.jpg?w=300&h=225)

## Result
![Panorama Result](https://ramsrigoutham.files.wordpress.com/2012/11/result_image1.jpg)

## Reference
Goutham, R. (2012, November 22). Panorama Image Stitching in Opencv. Retrieved from [https://ramsrigoutham.com/2012/11/22/panorama-image-stitching-in-opencv/](https://ramsrigoutham.com/2012/11/22/panorama-image-stitching-in-opencv/)
