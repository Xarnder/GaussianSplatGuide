# Gaussian Splat Guide
A guide on how to create Gaussian Splats for real-time applications 

<img src="media/Guassian Splat 2.PNG" height="400">

## Gausian Splat Introduction 
In the evolving landscape of mixed and virtual reality, the need for fully immersive, high detailed environments is great. Gaussian Splatting was a technique revitalised for real time rendering as of Siggraph 2023. This marked a pivotal advancement in the way we could view 3D data.

Unlike traditional rasterization methods that rely on a large array of vertices and faces, Gaussian Splatting offers a new way of representing 3D objects and scenes by applying the use of mathematical functions to represent 3D data. This approach, is deeply benefited by machine learning, to allow for  algorithm to optimise the gaussian representations to best represent the data while reducing the stress on the rendering system. This method allows for even high level of detail and realism at a lower cost to render times, greatly improving on convetional rendering techniques. 

Gaussian Slatting is best used for scenes and objects that require a high complexity of 3D geometry. It is especially better for environments that do not have smooth flat surfaces. This technology not only greatly enhances the visual fidelity or games and other VR and AR experiences but could also be an import part of immortalising  important culture and historical sites, by extracting key details of structure and representing them in high detail for anyone to view. The need for high detailed environments could also extend to educational or training purposes such as a way for fire fighters to safely practice entering and extinguishing a fire in a safe virtual reality application. Not to mention that gaussian splatting could be adapted further in the future to represent more than just still environments, but also moving animals and humans at a much higher level of detail then old methods for digital creature representation. 



## Guide to creating your own Gaussian Splats

## &nbsp;1.	Image Acquisition
<br>
### &nbsp;&nbsp;&nbsp;1.1 Take Photos
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   Start by capturing a series of images of your subject. Aim for a wide range of angles to get a comprehensive view.
<br>
### &nbsp;&nbsp;&nbsp;1.2   Recording Technique
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ideally, record a continuous video while walking around the subject. Keep your pace steady and even to ensure consistent angles throughout the scene.
<br>
### &nbsp;&nbsp;&nbsp;1.3 Focus on Details
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pay special attention to the undersides of objects, which are often missed at standard viewing heights.
<br>
### &nbsp;&nbsp;&nbsp;1.4 Control Motion Blur
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Maintain a moderate pace while recording to avoid motion blur, which could compromise the accuracy of your Gaussian Splat.
<br>
### &nbsp;&nbsp;&nbsp;1.5 Ensure Consistency
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ensure uniformity across all frames, fix your camera settings before starting. This includes the exposure, aperture, ISO, and focal length settings to avoid visual inconsistencies in the final product.
<br>
## 2.	Image Extraction and Preparation
 * Following the previous step is important that the format of the images is correct for the process to work properly. This can be efficiently accomplished by using a smartphone to record a video and then transferring the footage to an editing software such as Adobe Premiere Pro. You may need to attach a wire between your phone and computer and allow them to access each other's data. In Premier Pro adjust the export settings to conform to the preferred resolution of 980x545 pixels for this Gaussian Splatting Process. The next step is to Establish a precise naming convention for the image data set. Starting from “00001” and ascending sequentially, ensuring that each numerical name has 5 digits. The total number of images will directly influence the duration of the time needed to train the model. Approximately 500 images are a good number of images for this process. This can be achieved by slowing down or footage to a certain length and exporting a set frame rate. For example, if you want 500 images you could slow down your footage to 20 seconds and export your images at 25fps as a jpeg. Prepare toy dataset by also organising the images to a set file structure. Within a suitably named directory, create a directory inside it named ‘input’ folder. Then compress the folder into a zip archive for easier transfer later.
## 3. Image Data Set Upload
 * To progress to the next stage of this process you will need to login into your Google Drive and upload the zip file. Then navigate to the Google Colab at this link: colmap_gaussian_splatting_colab.ipynb - Colaboratory (google.com). At the top of the page press ‘copy to drive’ for personal access. The next stage involves linking your Google Drive to the Google Notebook. To do this create a new cell and input and run these commands.
## 4.	Model Training
 * Next click this [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qsrRkm4rLCxQGKGTpKqK7u_iHNLjGFRc?usp=sharing) button     After clicking the Colab link you'll see a code cell that has these lines at the top of it.
   ```
   zip_file_path = '/content/drive/MyDrive/nerf/'  # Path to the folder containing the zip file
   zip_file_name = 'lego.zip'  # Name of the zip file
   ```
   Change '/content/drive/MyDrive/nerf/' to point to folder containing your zip folder on your google drive.
   Then change 'lego.zip' to the name of your zip file



## Demo Video of Results
[Watch on YouTube]("https://youtu.be/jjLMmTkjSHk?si=26KtQf-sPShTw1zJ") <br>
<br>
[![Custom Thumbnail](https://github.com/Xarnder/GaussianSplatGuide/raw/main/media/Guassian%20Splat%2012.PNG)](https://youtu.be/jjLMmTkjSHk?si=6JiZsKZV7QIY5a5o)


scene credit: Bournemouth University Poole Gateway Desk [Bournemouth University NCCA](https://www.bournemouth.ac.uk/)

## About 
Guide based on the tool made by cclaan
- [Original Gaussian Splatting Tool by cclaan](https://github.com/laanlabs/metal-splats)
- [Original Gaussian Splatting Repo](https://github.com/graphdeco-inria/gaussian-splatting/)
- [Unity Gaussian Splatting](https://github.com/aras-p/UnityGaussianSplatting)
- [WebGL Gaussian Splats](https://github.com/antimatter15/splat)
- [WebGPU Gaussian Splatting from cvlab-epfl](https://github.com/cvlab-epfl/gaussian-splatting-web) 
- [MrNeRF gaussian splatting cuda](https://github.com/MrNeRF/gaussian-splatting-cuda)


Uses [Satin + Forge](https://github.com/Hi-Rez/Satin) for AR + 3d viewer ( by [@rezaali](https://twitter.com/RezaAli) )
 



## License(s)
Parts of the code are based on the original Gaussian-Splatting software and is governed by the [Gaussian-Splatting License](https://github.com/graphdeco-inria/gaussian-splatting/blob/main/LICENSE.md), which can be found in the [LICENSE]() file in this repository. The original software was developed by Inria and MPII.

Please be advised that the software in this repository cannot be used for commercial purposes without explicit consent from the original licensors, Inria and MPII.

[Satin + Forge](https://github.com/Hi-Rez/Satin) are released under the MIT license. See [LICENSE](https://github.com/Hi-Rez/Satin/blob/master/LICENSE) for details. 
