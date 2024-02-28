# Gaussian Splat Guide
A guide on how to create Gaussian Splats for real-time applications 

<img src="media/Guassian Splat 2.PNG" height="400">

## Gausian Splat Introduction 


## Guide to creating your own Gaussian Splats

1.	## Image Acquisition
 *	The procedure for Generating Gaussian Splat from Captured Imagery starts my at the Image Acquisition stage. Begin the process  by carefully capturing a series of images of the subject from a comprehensive range of angles. The most optimal way to do this involves recording a continuous video while circling the subject at a steady even pace, thus ensuring a uniform distribution of angles around the scene. Special attention should be paid to capturing the undersides of objects, which often are not seen from standard heights. Maintain a moderate speed to prevent motion blur, which can adversely affect the Gaussian Spat accuracy. Consistency across frames is vital, and so camera settings such as exposure, aperture, ISO and focal lengths should be fixed to eliminate visual artefacts in the final rendering process. 
3.	## Image Extraction and Preparation
 * Following the previous step is important that the format of the images is correct for the process to work properly. This can be efficiently accomplished by using a smartphone to record a video and then transferring the footage to an editing software such as Adobe Premiere Pro. You may need to attach a wire between your phone and computer and allow them to access each other's data. In Premier Pro adjust the export settings to conform to the preferred resolution of 980x545 pixels for this Gaussian Splatting Process. The next step is to Establish a precise naming convention for the image data set. Starting from “00001” and ascending sequentially, ensuring that each numerical name has 5 digits. The total number of images will directly influence the duration of the time needed to train the model. Approximately 500 images are a good number of images for this process. This can be achieved by slowing down or footage to a certain length and exporting a set frame rate. For example, if you want 500 images you could slow down your footage to 20 seconds and export your images at 25fps as a jpeg. Prepare toy dataset by also organising the images to a set file structure. Within a suitably named directory, create a directory inside it named ‘input’ folder. Then compress the folder into a zip archive for easier transfer later.
4.	## Image Data Set Upload
 * To progress to the next stage of this process you will need to login into your Google Drive and upload the zip file. Then navigate to the Google Colab at this link: colmap_gaussian_splatting_colab.ipynb - Colaboratory (google.com). At the top of the page press ‘copy to drive’ for personal access. The next stage involves linking your Google Drive to the Google Notebook. To do this create a new cell and input and run these commands. 


This allows for direct manipulation of the data set within the Collab Environment.



Next click this
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qsrRkm4rLCxQGKGTpKqK7u_iHNLjGFRc?usp=sharing) button
<br>
After clicking the Colab link you'll see a code cell that has these lines at the top of it.
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
