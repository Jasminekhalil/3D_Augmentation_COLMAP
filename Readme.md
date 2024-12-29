# Offline 3D Augmentation Using COLMAP

This project describes the development of an **Augmented Reality (AR) Viewer** capable of overlaying virtual objects onto images of real-world scenes. Our **offline implementation** integrates concepts from **computer vision, computer graphics, and geometry.** 

Using **COLMAP software** for **3D reconstruction**, we generated a **sparse 3D point cloud** from overlapping camera image views. The key tasks completed include extracting the **dominant plane** using a custom **RANSAC algorithm**, **transforming coordinate systems**, and projecting a virtual 3D object onto 2D images using camera parameters. This project emphasizes foundational mathematical techniques, such as **camera projection and geometric transformations**, with a focus on implementing core algorithms without relying on external computer vision libraries. Our work provides a **solid basis for future real-time AR applications.**

---

## Steps Taken

1. We first captured a set of overlapping images of a 3D scene and used COLMAP to generate a sparse 3D point cloud. 
2. We then developed and implemented a RANSAC algorithm to identify the dominant plane within the scene.
3. After that, we defined a local coordinate system for placing a virtual object.
4. Then, we created a virtual 3D object, transformed it to fit the scene’s geometry, and projected it onto the original images using the pinhole camera model based on internal and external camera parameters.
5. Finally, we rendered the image
views with the virtual object accurately overlaid, achieving an
offline AR viewer.

---

## Initial Views of our Chosen Scene 

![View 1](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/image1.JPG)
![View 2](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/image2.JPG)
![View 3](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/image3.JPG)
![View 4](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/image4.JPG)
![View 5](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/image5.JPG)
![View 6](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/image6.JPG)

---

## COLMAP 3D Reconstruction

![COLMAP Reconstruction](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/colmapreconstruction.png)

---

## Dominant Plane of our Scene from RANSAC Algorithm

![Plot of all points and inliers accurately identifying our dominant plane](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/dominantplane.png)


## 3D Euclidean transformation of 3D Box onto the Dominant Plane

![Plot of 3D box accurately placed at the center of the dominant plane.](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/3Dscenewithbox.png)

--- 

## Views of our Chosen Scene with the 3D Box Projected Onto the Real Scene

![View 1](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/pinkbox1.png)
![View 2](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/pinkbox2.png)
![View 3](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/pinkbox3.png)
![View 4](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/pinkbox4.png)
![View 5](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/pinkbox5.png)
![View 6](https://github.com/Jasminekhalil/3D_Augmentation_COLMAP/blob/main/Results/pinkbox6.png)

- **Email**: [jasminekhalil213@gmail.com](mailto:jasminekhalil213@gmail.com)  
- **LinkedIn**: [JasmineKhalil21](https://www.linkedin.com/in/jasminekhalil21/)