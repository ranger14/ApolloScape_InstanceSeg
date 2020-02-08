# EfficientNet - 6DVNet / ApolloScape_InstanceSeg

This is an ApolloScape_InstanceSeg (or 6DVNet) library from stevenwudi with EfficientNet as the backbone.

### About EfficientNet

If you're new to EfficientNets, here is an explanation straight from the official TensorFlow implementation: 

EfficientNets are a family of image classification models, which achieve state-of-the-art accuracy, yet being an order-of-magnitude smaller and faster than previous models. We develop EfficientNets based on AutoML and Compound Scaling. In particular, we first use [AutoML Mobile framework](https://ai.googleblog.com/2018/08/mnasnet-towards-automating-design-of.html) to develop a mobile-size baseline network, named as EfficientNet-B0; Then, we use the compound scaling method to scale up this baseline to obtain EfficientNet-B1 to B7.

<table border="0">
<tr>
    <td>
    <img src="https://raw.githubusercontent.com/tensorflow/tpu/master/models/official/efficientnet/g3doc/params.png" width="100%" />
    </td>
    <td>
    <img src="https://raw.githubusercontent.com/tensorflow/tpu/master/models/official/efficientnet/g3doc/flops.png", width="90%" />
    </td>
</tr>
</table>

EfficientNets achieve state-of-the-art accuracy on ImageNet with an order of magnitude better efficiency:


* In high-accuracy regime, our EfficientNet-B7 achieves state-of-the-art 84.4% top-1 / 97.1% top-5 accuracy on ImageNet with 66M parameters and 37B FLOPS, being 8.4x smaller and 6.1x faster on CPU inference than previous best [Gpipe](https://arxiv.org/abs/1811.06965).

* In middle-accuracy regime, our EfficientNet-B1 is 7.6x smaller and 5.7x faster on CPU inference than [ResNet-152](https://arxiv.org/abs/1512.03385), with similar ImageNet accuracy.

* Compared with the widely used [ResNet-50](https://arxiv.org/abs/1512.03385), our EfficientNet-B4 improves the top-1 accuracy from 76.3% of ResNet-50 to 82.6% (+6.3%), under similar FLOPS constraint.

# Instance segmentation 


[ApolloScene Understanding](http://apolloscape.auto/scene.html) 

Steps:

* [Trainining](#trainining)
* [Testing](#testing)


## Implementation details

### Trainining:  `train_net_step.py`
This step will first collect ROI from the function 
`combined_roidb_for_training`



### Testing
`test_net_WAD.py`



## Citation

I would appreciate citation of the following paper if you find this repository helpful.

```
@InProceedings{Wu_2019_CVPR_Workshops,
author = {Wu, Di and Zhuang, Zhaoyong and Xiang, Canqun and Zou, Wenbin and Li, Xia},
title = {6D-VNet: End-To-End 6-DoF Vehicle Pose Estimation From Monocular RGB Images},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2019}
```
