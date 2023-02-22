
# ROAD-Agents-Detection

## Data Setup

If you are using your local system, please download `ROAD-Agent-Detection` from [our Google-Drive](https://drive.google.com/drive/folders/1Y1XcSpdMU-vHnF_RjwQ-XAgJ2ovGBk61?usp=share_link)

Alternatively, you can create a shortcut of the [Google-Drive folder `ROAD-Agent-Detection`](https://drive.google.com/drive/folders/1Y1XcSpdMU-vHnF_RjwQ-XAgJ2ovGBk61?usp=share_link) and load it to your google colab using [connect_gdrive.ipynb](./connect_gdrive.ipynb).

## Data splits

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

## Data formats

The ROAD dataset for object (agnet) detection is provided into three different formats:

### YOLO



### COCO

### Pascal-VOC


## Training Object Detectors


