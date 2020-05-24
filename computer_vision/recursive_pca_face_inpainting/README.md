# Recursive PCA Face Inpainting

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abeytheo/tinkering-ml/blob/master/computer_vision/recursive_pca_face_inpainting/recursive_pca_face_inpainting.ipynb)

Given a masked image, the goal of the recursive PCA algorithm is to fill in the missing region with appropriate pixels retrieved from the eigenface space. In this project, I present three main topics:

- Basic face reconstruction using PCA
- PCA face reconstruction on RGB channel
- Face inpainting using recursive PCA

![recursive pca face inpaintiing](asset/recpca.png)

This project is inspired by a paper by Wang et al.

    @inproceedings{4425497,
      author={Z. {Wang} and J. {Tao}},
      booktitle={2007 International Conference on Computational Intelligence and Security Workshops (CISW 2007)}, 
      title={Reconstruction of Partially Occluded Face by Fast Recursive PCA}, 
      year={2007},
      volume={},
      number={},
      pages={304-307},
    }