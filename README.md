# Gaussian Splat Guide
A guide on how to create Gaussian Splats for real-time applications 

<img src="media/Guassian Splat 2.PNG" height="400">

## Gausian Splat Introduction 


## Guide to create your own gaussian splats

Next click the Open in Colab button bellow
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qsrRkm4rLCxQGKGTpKqK7u_iHNLjGFRc?usp=sharing) 
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
