## SphereSR: 360 Image Super-Resolution with Arbitrary Projection via Continuous Spherical Image Representation
##### Research Question
How to super resolve a 360 image under an arbitrary projection types and scales without quality degradation?

How to solve the inherent distortion and density difference issue in 360 images preojection in super resolution task?
##### Motivation
1. The angular resolution of a 360 image is lower than that of a narrow field-of-view(FOV) perspective image as it is captured using fisheye lenses with the same sensor size.
2. Most existing methods consider the ERP as the representation of the input and output and ignore the projection process of 360 images, however, another information loss may occur when transforming the HR image to other projection types.
3. Existing 2D SR methods are less applicable for 360 images represented in 2D planar representation as the pixel density and texture complexity are various cross different latitudes.

##### Method
1. To solve the ERP image distortion problem and the pxel density difference according to the latitude.
A feature extraction module

##### Experiments

##### Good Expression
- Thus, it is vital to address the ERP distortions problems and strive to super-resolve an ODI image to an HR image with an arbitrary projection type rather than a fixed type.


## SpherePHD: Applying CNNs on a Spherical PolyHeDron Representation of 360 Images
##### Research Question
How to solve the difficulty of projection distortion and discontinuity issues when applying CNN in omni-directional images failing to extract meaningful information?
##### Motivation
1. The input of convolutional neural networks are usually represented in the Euclidean space, however, the original representation of omni-directional images are in non-Euclidean space, which result in the spatial distortion when we want to transform the representtaion type in Euclidean like ERP.
2. The transformation from non-Euclidean space to Euclidean space result in the continuity and cyclical properties disappearance. Even though, the cube map representation can somehow alleviate the distortion issue, it is still difficult to extract uniform locality information on the top and bottom faces because the top and bottom faces of cube map are orthogonal to the other faces.
##### Method
- Data Structure

  **Project the omni-directional image onto an icosahedral spherical polyhedron**

<img src="Snipaste_2022-09-08_20-53-08.png" width="60%" />

  - **Why this representation ?**
  
    Because it has far less irregularity on an input image.
    
    Here, the paper defines the average effective area of all the pixels as 
  
- Convolution layer
- Pooling layer
##### Good Expression
