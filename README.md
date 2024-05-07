This project focuses on the computing homographies and designed to seamlessly stitch images together to create stunning panoramic views. This project utilizes advanced computer vision techniques and algorithms to achieve precise image alignment and blending, resulting in a seamless and immersive panoramic experience. Below are the key steps involved in the Panoramic Fusion process:

### Final Result
![output](https://github.com/tathya7/Panormaic-Fusion/assets/105652825/26a6c34e-3933-4828-a7df-6ec0bb3c0b0c)




#### 1. Feature Matching with SIFT and FLANN

- Two input images are taken, and their respective features and descriptors are extracted using the Scale-Invariant Feature Transform (SIFT) algorithm.
- The FLANN (Fast Library for Approximate Nearest Neighbors) algorithm is then used to match the keypoints between the two images.
- Matching keypoints are visually represented by drawing lines or markers on the images, showcasing the correspondence between key features.

![image](https://github.com/tathya7/Panormaic-Fusion/assets/105652825/a52a84f1-d1ae-4011-be6f-e3691126d7a0)


#### 2. Homography Computation and Perspective Transformation

- Homographies are computed based on the matched keypoints, establishing the geometric transformation between the images.
- Using the computed homographies, one image is warped to align with the perspective of the other image, ensuring seamless integration.


#### 3. Blending the images & Stitching Images

- To create a natural and visually appealing fusion, the warped images are blended together using advanced blending techniques.
- The blending process ensures smooth transitions between overlapping regions
- For stitching multiple images into a panoramic view, a blank canvas of the final combined image's dimensions is created.
- Each stitched image is accurately placed and pasted onto this canvas, aligning them based on the computed homographies.



