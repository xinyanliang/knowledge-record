# Recommended Papers ![Maintenance](https://img.shields.io/maintenance/yes/2017.svg) [![DUB](https://img.shields.io/dub/l/vibe-d.svg)](LICENSE)
## [Home](../README.md)
- 记录经典的深度学习模型.

[tensorflow](https://github.com/tensorflow)实现[model](https://github.com/tensorflow/models/tree/master/research/slim)
## Papers
Paper list.

## Image Captioning
|No.  |Figure   |Net Name |Title   |Authors  |Pub.  |Links|
|-----|:-----:|:-----:|:-----:|:-----:|:---:|:---:|
|1|![Smile](netimage/LeNets.png)|LeNet|__Gradient-based learning applied to document recognition__|Cesc Chunseong Park, Byeongchang Kim and Gunhee Kim|__Proceedings of the IEEE 1998__|[PDF](http://yann.lecun.com/exdb/publis/pdf/lecun-98.pdf) [Project](http://yann.lecun.com/exdb/lenet/)  解读|
|2|![Smile](netimage/Alexnet.png)|AlexNet|__ImageNet Classification with Deep Convolutional Neural Networks__|Cesc Chunseong Park, Byeongchang Kim and Gunhee Kim|__NIPS2012__|[PDF](http://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)  解读|
|3|![Smile](netimage/ZFnet.png)|ZF-net|__Visualizing and understanding convolutional networks__|[Matthew D Zeiler](http://www.matthewzeiler.com/) and [Rob Fergus](http://cs.nyu.edu/~fergus/pmwiki/pmwiki.php)|__ECCV2014__|[PDF](https://arxiv.org/pdf/1311.2901.pdf)  解读|
|4|![Smile](netimage/VGG.png)| VGG|__Very deep convolutional networks for large-scale image recognition__|Cesc Chunseong Park, Byeongchang Kim and Gunhee Kim|__ICLM2015__|[PDF](http://www.robots.ox.ac.uk/~vgg/research/very_deep/) [code](https://github.com/cesc-park/attend2u) 解读|
|5|![Smile](netimage/Inception1.png)| GoogLeNet|__Going deeper with convolutions__|Christian Szegedy, Wei Liu, Yangqing Jia, Pierre Sermanet, Scott Reed, Dragomir Anguelov, Dumitru Erhan, Vincent Vanhoucke, Andrew Rabinovich|__CVPR2015__|[PDF](https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Szegedy_Going_Deeper_With_2015_CVPR_paper.html) [code](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v1.py) 解读|
|6|![Smile](netimage/Inceptionv2.png)| Inception v2|__Batch normalization: Accelerating deep network training by reducing internal covariate shift__|Cesc Chunseong Park, Byeongchang Kim and Gunhee Kim|__ICML2015__|[PDF](https://arxiv.org/abs/1502.03167) [code](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v2.py) 解读|
|7|![Smile](netimage/Inceptionv3.png)| Inception-v3|__Rethinking the inception architecture for computer vision__|Cesc Chunseong Park, Byeongchang Kim and Gunhee Kim|__CVPR2016__|[PDF](https://arxiv.org/abs/1512.00567) [code](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v3.py) 解读|
|7|![Smile](netimage/Inception4.png)| Inception-v4|__Inception-v4, inception-resnet and the impact of residual connections on learning__|Cesc Chunseong Park, Byeongchang Kim and Gunhee Kim|__AAAI2017__|[PDF](https://arxiv.org/abs/1602.07261) [code](https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v4.py) 解读|
|8|![Smile](netimage/ResNet.png)| ResNets|__Deep residual learning for image recognition__|Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun|__CVPR2016__|[PDF](https://www.cvfoundation.org/openaccess/content_cvpr_2016/html/He_Deep_Residual_Learning_CVPR_2016_paper.html) [github](https://github.com/KaimingHe/deep-residual-networks) 解读|
|9|![Smile](netimage/ResNetsv2.png)| ResNets|__Identity mappings in deep residual networks__|Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun|__ECCV2016__|[PDF](https://arxiv.org/abs/1603.05027) [code](https://github.com/facebook/fb.resnet.torch) 解读|
|10|![Smile](netimage/densenet.jpg)| DenseNets|__Densely Connected Convolutional Networks__|[Huang, Gao](http://www.cs.cornell.edu/~gaohuang/) and [Liu, Zhuang](https://liuzhuang13.github.io/) and, [Laurens van der Maaten](https://lvdmaaten.github.io/), [Kilian Q Weinberger](https://www.cs.cornell.edu/~kilian/)|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/pdf/1608.06993.pdf) [github](https://github.com/liuzhuang13/DenseNet) 解读|
|11|![Smile](netimage/PyramidNet.png)| DenseNets|__Deep Pyramidal Residual Networks__|Dongyoon Han, Jiwhan Kim, Junmo Kim|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/pdf/1610.02915.pdf) [github](https://github.com/jhkim89/PyramidNet) 解读|
|12|![Smile](netimage/FPNt.png)| FPN|__Feature Pyramid Networks for Object Detection__|Tsung-Yi Lin, Piotr Dollár, [Ross Girshick](Ross Girshick (rbg)), [Kaiming He](http://kaiminghe.com/), Bharath Hariharan, and Serge Belongie|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/pdf/1612.03144.pdf) [github]() 解读|
|13|![Smile](netimage/ResNeXt.png)| ResNeXt|__Aggregated Residual Transformations for Deep Neural Networks__|Saining Xie, Ross Girshick, Piotr Dollár, Zhuowen Tu, Kaiming He|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/abs/1611.05431) [github](https://github.com/facebookresearch/ResNeXt) 解读|
|14|![Smile](netimage/DRNs.png)| DRNs|__Dilated Residual Networks__|[Fisher Yu](http://www.yf.io/), Vladlen Koltun, Thomas Funkhouser|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/abs/1705.09914) [github](https://github.com/fyu/drn)| 解读|
|15|![Smile](netimage/MobileNets.png)| MobileNets|__MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications__|Andrew G. Howard, Menglong Zhu, Bo Chen, Dmitry Kalenichenko, Weijun Wang, Tobias Weyand, Marco Andreetto, Hartwig Adam|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/pdf/1704.04861.pdf) [github](https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet_v1.py)| 解读|
|16|![Smile](netimage/SqueezeDet.png)| __SqueezeDet__|__SqueezeDet: Unified, Small, Low Power Fully Convolutional Neural Networks for Real-Time Object Detection for Autonomous Driving__|Bichen Wu, Forrest Iandola, Peter H. Jin, Kurt Keutzer|__[CVPR2017](http://www.cvpapers.com/cvpr2017.html)__|[PDF](https://arxiv.org/abs/1612.01051) [github](https://github.com/BichenWuUCB/squeezeDet)| 解读|
|17|![Smile](netimage/DCNs.png)| __DCNs__|__Multi-Scale Context Aggregation by Dilated Convolutions__|[Fisher Yu](http://www.yf.io/), Vladlen Koltun|__ICLR2016__|[PDF](https://arxiv.org/abs/1511.07122) [github](https://github.com/fyu/dilation)| 解读|




 


 

