# Gaussian Splat Guide
A guide on how to create Gaussian Splats for real-time applications 

<img src="media/Guassian Splat 2.PNG" height="400">

## Guide to create your own gaussian splats
There are several [blog posts](https://www.reshot.ai/3d-gaussian-splatting) on how to train your own models from a set of images. 
The output PLY model is what you want to keep ( e.g. 'iteration_30000/point_cloud.ply' ) 
The included models were trained on google colab with an A100 GPU. 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1I8T2zlE7fQK06uNfezr4tOa_5xSq9XIg?usp=sharing) 

## Demo Video of Results
[Watch on YouTube](https://youtu.be/2th0ejgNu4U) <br>
[![youtube-link](https://github.com/laanlabs/metal-splats/assets/174185/5b73c660-8466-4b5d-b68d-2a44c0d1aff5)](https://youtu.be/2th0ejgNu4U)

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
