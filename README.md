# Anno-Mage: A Semi Automatic Image Annotation Tool

![alt text](https://raw.githubusercontent.com/virajmavani/semi-auto-image-annotation-tool/master/demo.gif)

Semi Automatic Image Annotation Toolbox with RetinaNet as the suggesting algorithm. The toolbox suggests 80 class objects from the MS COCO dataset using a pretrained YoLov5 model (https://github.com/ultralytics/yolov5).
This repo is modified from https://github.com/opencvfun/semi-auto-image-annotation-tool

## Installation

1) Clone this repository.

2) In the repository, execute `pip install -r requirements.txt`

3) Download the yolov5 pretrained weights: 
```bash
sh yolov5/weights/download_weights
```

### Instructions

1) Select (Remove) the COCO object classes for which you do not need suggestions from the class panel (right-down panel).

2) When annotating manually, select the object class from the List and while keep it selected, select the BBox.

3) The final annotations can be found in the file `annotations.csv` in ./annotations/

### Usage
```
python main.py
```


### Example

Open the software by:
```
python main.py
```

Select image dir or image as 'yolov5/inference/images/bus.jpg' or 'yolov5/inference/images'

Start annotating and check the annotations in 'annotations' folder!
 
 
### Others
Tested on:

1. Windows 10

2. Linux 16.04

3. macOS High Sierra

### Acknowledgments

1) [Meditab Software Inc.](https://www.meditab.com/)

2) [Keras implementation of RetinaNet object detection](https://github.com/fizyr/keras-retinanet)

3) [Computer Vision Group](https://cvgldce.github.io/), L.D. College of Engineering
