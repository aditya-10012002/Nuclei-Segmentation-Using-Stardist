<h1 align="center">Nuclei-Segmentation-Using-Stardist</h1>
<p align="center">NUCLEI SEGMENTATION  USING STARDIST AND PYTHON IN GOOGLE COLAB</p>

<p align="center">
  <img src="https://github.com/aditya-10012002/Nuclei-Segmentation-Using-Stardist/assets/53975591/8a36c8ea-c8e9-471c-8722-bf961b024cfd" alt="Plot">
</p>

## Problem Statement

We are provided with a dataset of cells (nuclei) containing a total of 28 images which are to
be segmented, analyzed and finally documented. In this report, I have put in a detailed
analysis of the segmentation result and the images (Original, Segmented, Merged) are
provided in a zip file.
## Procedure
### Model

We start with aggregating all the images to simplify further processes. Then we use the
pre-trained model “Versatile (fluorescent nuclei)” from the stardist package since it’s one of
the best for monochromatic images. Using the stardist segmentation function, we store the
segmented image per input image. After this step, we proceed to plot one as an example
(refer colab notebook).

### Centroid and Annotation

We then proceed to calculate the centroid coordinates of all the cells and store them in a
variable “features” to use in the further steps. Using that, we annotate it graphically as
shown.
</br>
<p align="center">
  <img src="https://github.com/aditya-10012002/Nuclei-Segmentation-Using-Stardist/assets/53975591/98c22029-70a2-45e4-9148-3755e0cd09d4" alt="Annotation">
</p>


### Trajectory and Drift

We then use Bubble tracking to plot the trajectories of the nuclei spanning across all the
images. We then proceed to calculate the overall drift and using that, plot the corrected
trajectories as shown below.
</br>
<p align="center">
  <img src="https://github.com/aditya-10012002/Nuclei-Segmentation-Using-Stardist/assets/53975591/2744d66c-5faf-49a0-9863-cc7c5315e913" alt="Trajectory">
</p>
<p align="center">Trajectory</p>

<p align="center">
  <img src="https://github.com/aditya-10012002/Nuclei-Segmentation-Using-Stardist/assets/53975591/e1c3fcb6-7e19-4605-9b5c-9ec020eb89a8" alt="Drift">
</p>
<p align="center">Overall Drift</p>

<p align="center">
  <img src="https://github.com/aditya-10012002/Nuclei-Segmentation-Using-Stardist/assets/53975591/ce5d1ff2-aa86-437e-8fad-633b0a777814" alt="Corrected Trajectory">
</p>
<p align="center">Corrected Trajectory</p>



## Result

After doing the analysis, we finally plot the results as follows:
The images are present in the zip attached.
Can also access here - https://drive.google.com/drive/folders/1fuidbbXZidS5g0Vw0A_K1EFX6MC9Gj-d?usp=sharing
