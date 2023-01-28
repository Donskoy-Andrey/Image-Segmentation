# The Problem
Segment images of skin neoplasms from ADDI Project dataset using one of 
of the proposed methods (Graph-based segmentation, Normalized cuts, convolutional neural networks). 
We used convolutional neural networks as the solution. 

When using neural networks, the sample is divided into a 100/50/50 ratio.
The quality of the model is evaluated using the IoU (Intersection over Union) metric.

# Results
SegNet and U-Net architectures with 3 loss functions were built: BCE, Dice, Focal. In total all 6 structures were trained on 300 epochs.\
The results of the metrics, as well as the graphs of change in the loss are presented in the SegNet (Summary) and U-Net (Summary) blocks:

<p align="center">
  <img src="https://github.com/Donskoy-Andrey/Image-Segmentation/blob/master/images/segnet.png" />
  <img src="https://github.com/Donskoy-Andrey/Image-Segmentation/blob/master/images/unet.png" />
</p>

# Metric Value
The best model obtained is SegNet at Focal Loss, the metric result is **0.792 at 240 epoch.**

## Competition Result
> 79/100 points, 7th place in the top. [Winner's diploma](https://github.com/Donskoy-Andrey/Image-Segmentation/blob/master/images/Диплом.pdf).
