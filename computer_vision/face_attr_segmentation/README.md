# Face Attribute Segmentation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abeytheo/tinkering-ml/blob/master/computer_vision/face_attr_segmentation/face_attribute_segmentation.ipynb)

Given some segmentation labels, a face attribute segmentation model is trained to predict pixels contained in an image with respect to their corresponding segment labels. In this project, [Helen Face Dataset](http://pages.cs.wisc.edu/~lizhang/projects/face-parsing/) is used to train the segmentation model. Furthermore, the model uses UNet encoder-decoder architecture with Adam optimizer. I encountered an imbalanced dataset problem, thus, it is trained by using a weighted cross entropy loss. IoU as well as individual class precision and recall become the chosen evaluation metric.

![face attr segmentation ](asset/face_attr_segmentation.png)

Some of the key ideas were based on [a paper by Kalayeh et al.](https://www.crcv.ucf.edu/papers/cvpr2017/Kalayeh_CVPR2017.pdf). In addition, the dataset used in this project is authored by [Smith et al.](http://pages.cs.wisc.edu/~lizhang/projects/face-parsing/SmithCVPR2013.pdf)

    @InProceedings{Kalayeh_2017_CVPR,
      author = {Kalayeh, Mahdi M. and Gong, Boqing and Shah, Mubarak},
      title = {Improving Facial Attribute Prediction Using Semantic Segmentation},
      booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
      month = {July},
      year = {2017}
    }

    @inproceedings{10.1109/CVPR.2013.447,
      author = {Smith, Brandon M. and Zhang, Li and Brandt, Jonathan and Lin, Zhe and Yang, Jianchao},
      title = {Exemplar-Based Face Parsing},
      year = {2013},
      url = {https://doi.org/10.1109/CVPR.2013.447},
      booktitle = {Proceedings of the 2013 IEEE Conference on Computer Vision and Pattern Recognition},
      series = {CVPR ’13}
    }


