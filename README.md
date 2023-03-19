
# ROAD-Agents-Detection

## Data Setup

If you are using your local system, please download `ROAD-Dataset` from [our Google-Drive](https://drive.google.com/drive/folders/1Y1XcSpdMU-vHnF_RjwQ-XAgJ2ovGBk61?usp=sharing)

Alternatively, you can create a shortcut of the [Google-Drive folder `ROAD-Dataset`](https://drive.google.com/drive/folders/1Y1XcSpdMU-vHnF_RjwQ-XAgJ2ovGBk61?usp=sharing) and load it to your google colab using [connect_gdrive.ipynb](./connect_gdrive.ipynb).

## Data Splits

The dataset is divided into three splits; train_set, val_set, and test_set

```
    ROAD-Dataset/
        - train_set.json
        - train_set/
            - 2014-06-25-16-45-34_stereo_centre_02_00001.jpg
            - 2014-06-25-16-45-34_stereo_centre_02_00001.txt
            - 2014-06-25-16-45-34_stereo_centre_02_00001.xml
            - ........

        - val_set.json
        - val_set/
            - 2014-06-26-09-53-12_stereo_centre_02_00001.jpg
            - 2014-06-26-09-53-12_stereo_centre_02_00001.txt
            - 2014-06-26-09-53-12_stereo_centre_02_00001.xml
            - ........

        - test_set.json
        - test_set/
            - 2014-06-26-09-31-18_stereo_centre_02_00001.jpg
            - 2014-06-26-09-31-18_stereo_centre_02_00001.txt
            - 2014-06-26-09-31-18_stereo_centre_02_00001.xml
            - ........

```

## Data Formats

The ROAD dataset for object (agnet) detection is provided into three different formats:

### YOLO

In the yolo format, the annotation is provided in txt file where for each of the image there should be a txt file with the same name (as shown in data splits).

### COCO

In coco format, the annotation is provided in a json file where for each of the split (diretory) there should be a json file having the annotations for all the split.

### Pascal-VOC

In the Pascal-Voc format, the annotation is provided in xml file where for each of the image there should be an xml file with the same name (as shown in data splits).

## Training Object Detectors

As examples, we provided links to object detectors (one from each above formats).

### YOLO -- Following YOLO format

YOLO object detection family has 8 different versions, one of the most famous version is YOLOv5.

YOLOv5 can be install from this link https://github.com/ultralytics/yolov5.

To train your ROAD-Agents-Detection you need to follow the instruction given in this link https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data. The data and yml file are already provided in the desired format.


### Mmdetection Library -- Following COCO format

MMDetection is an open source object detection toolbox based on PyTorch.

Mmdetection library can be install from this link https://github.com/open-mmlab/mmdetection.

To train any object detector from mmdetection library you need to follow the instruction given in this link https://github.com/open-mmlab/mmdetection/blob/master/docs/en/2_new_data_model.md. The data and json files are already provided in the desired format.


### TensorFlow Object Detection API

TensorFlow Object Detection API is also an open source object detection toolbox based on TensorFlow.

TensorFlow Object Detection API can be install from this link https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2.md.

To train any object detector from TensorFlow Object Detection API you need to follow the instruction given in this link https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_training_and_evaluation.md. The data is provided in Pascal Voc format (images and xml files), which needs to be convert into tfrecord by following the instructions in this link https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/preparing_inputs.md
