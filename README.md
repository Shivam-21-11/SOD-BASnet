# BASNet: Boundary-Aware Salient Object Detection

- Deep Convolutional Neural Networks have been adopted for salient object detection and achieved the state-of-the-art performance. Most of the previous works however focus on region accuracy but not on the boundary quality.
- In this project, we propose a predict-refine architecture, BASNet, and a new hybrid loss for Boundary-Aware Salient object detection. Specifically, the architecture is composed of a densely supervised Encoder-Decoder network and a residual refinement module, which are respectively in charge of saliency prediction and saliency map refinement.
- The Research paper referred  is [BASNet: Boundary-Aware Salient Object Detection](https://openaccess.thecvf.com/content_CVPR_2019/papers/Qin_BASNet_Boundary-Aware_Salient_Object_Detection_CVPR_2019_paper.pdf "BASNet: Boundary-Aware Salient Object Detection") 

## Objective 
- The Official Code for the Basnet Model is provided by the authors on the [github](https://github.com/xuebinqin/BASNet "github").
- The Official Deep Learning model is made using Pytorch , my Goal is to create a similar model using tensorflow.
- Why ? Whilst Pytorch provide better developer experience and error handeling, I find Tensorflow to be a great ML Framework to work with for Beginners .  
- So the objective for this repo is to create Basnet Model using Tensorflow.

## Architecture
- The Architecture Proposed by the authors is predict-refine architecture.
- The Author have used  Transfer Learning  to improve model performance . They Used First 4 layers of the resnet34 model which is pretrained in imagenet dataset.
- But for the sake of understanding abstract architecture of the Basnet model I haven't used the transfer learning method , instead created each layer individually.

## Loss
- The hybrid loss guides the network to learn the transformation between the input image and the ground truth in a three-level hierarchy – pixel-, patch- and map- level – by fusing Binary Cross Entropy (BCE), Structural SIMilarity (SSIM) and Intersectionover- Union (IoU) losses.
## Thank You 
- This is my attempt to build the Basnet model using the research paper . If you find any error or mistakes let me know . Love all the feedbacks.
