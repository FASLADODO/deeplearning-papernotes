## [Mask R-CNN](https://arxiv.org/abs/1703.06870)

#### Key words
- instance segmentation, object detection, Faster R-CNN

#### Key points
- Authors present Mask-RCNN, simple, flexible, and general framework for object instance segmentation
- Mask R-CNN extends Faster R-CNN by adding a new branch for predicting an object mask in parallel with the existing branch for bounding box recognition
- Key features of Mask-RCNN
	- ROI Align: this removes harsd quantization of ROIPool
	- The mask and class prediction are decoupled by computing the loss of mask prediction only for the mask belonging to the ground truth class
	- Mask is generated by applying FCN to the each ROI
- Mask R-CNN can run 195ms per image on an NVIDIA Tesla M40 GPU
- Mask R-CNN can easily be extended even to key point detection task like human pose estimation

#### Thoughts
