
# ROAD-Agents-Detection

## Data Setup

If you are using your local system, please download `ROAD-Dataset` from [our Google-Drive](https://drive.google.com/drive/folders/1Y1XcSpdMU-vHnF_RjwQ-XAgJ2ovGBk61?usp=sharing)

Alternatively, you can create a shortcut of the [Google-Drive folder `ROAD-Dataset`](https://drive.google.com/drive/folders/1Y1XcSpdMU-vHnF_RjwQ-XAgJ2ovGBk61?usp=sharing) and load it to your google colab using [connect_gdrive.ipynb](./connect_gdrive.ipynb).

## Data Splits

The dataset is divided into three splits; train_set, val_set, and test_set

```
    ROAD-Agent-Detection/
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

