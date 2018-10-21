# DeepLab_V3_plus : a model about semantic segmentation
This is a simple pytorch re-implementation of Google [Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation](https://arxiv.org/pdf/1802.02611.pdf).

### Introduction:
This work still need to be updated.
The features are summarized blow:
+ Use ResNet101 as base Network.
+ Use only Pascal Voc 2012 for base dataset.


### We have finished:
+ Dataloader for [Pascal Voc 2012](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/).
+ You can check your dataloader error in 'path/to/workspace/check/check_dataloader/img'.
  You will see three part:
  + 1.original image which we load directly from image path.
  + 2.restore image from torch-tensor(transformed from numpy) back to numpy ndarray.
  + 3.mask loaded by dataloader.
  e.g.
  1. original.
  <div align=left><img width="300" height="300" src="https://github.com/songdejia/deeplab_v3_plus/blob/master/screenshot/original.png"/></div>

  2. restore image from tensor to numpy.
  <div align=left><img width="300" height="300" src="https://github.com/songdejia/deeplab_v3_plus/blob/master/screenshot/restore.png"/></div>

  3. mask
  <div align=left><img width="300" height="300" src="https://github.com/songdejia/deeplab_v3_plus/blob/master/screenshot/mask.png"/></div>
