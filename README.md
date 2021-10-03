# Pose Detection
This repository holds the tensorflow implementation of Single Person Pose Detection using Movenet and Apache MXNet implementation of Multi-Person Pose Detection using Openvino in Python.
<br>
## Dataset
The model 'Movenet' is trained on <a href="https://voxel51.com/docs/fiftyone/user_guide/dataset_zoo/index.html">MS COCO dataset.</a><br>
The model 'ssd_512_mobilenet1.0_coco' which is an object detection framework under OpenVino is trained on <a href="https://www.kaggle.com/zaraks/pascal-voc-2007">VOC2007</a>, <a href="https://www.kaggle.com/huanghanchina/pascal-voc-2012">VOC2012</a> and <a href="https://voxel51.com/docs/fiftyone/user_guide/dataset_zoo/index.html"> MS COCO</a> dataset. 
<br>

## Steps involved
### Single Person Pose Detection
- Imported the necessary libraries as mentioned in the 'Requirements' section.
- Defined the 'Movenet' model.
- Defined the function for drawing the landmarks and initialized the edges.
- Ran inference for pose detection using opencv.
<br>

### Multi-Person Pose Detection
- Imported the necessary libraries as mentioned in the 'Requirements' section.
- Defined the 'ssd_512_mobilenet1.0_coco' model for object detection.
- Modified the detector model such that it is made to detect only 'human beings'.
- Defined the 'simple_pose_resnet18_v1b' model for pose detection.
- Ran inference for pose detection using opencv. 

## Requirements

numpy==1.21.0
<br>
opencv-python==4.5.3
<br>
tensorflow==2.5.0
<br>
matplotlib==3.4.2
<br>
future==0.18.2
<br>
mxnet==1.8.0
<br>
gluoncv=0.10.4
<hr>

## Demo Video
### Single Person Pose Detection
https://www.youtube.com/watch?v=pVcm9asUgZg
<br>

### Multi-Person Pose Detection
