# Bird Classification

## Get data

Download the [dataset](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) and unpack it to `CNNs`. The directory should look like

```bash
-- CNNs
   |-- CUB_200_2011
   |    └── CUB_200_2011
   |    |   ├── attributes
   |    |   ├── bounding_boxes.txt
   |    |   ├── classes.txt
   |    |   ├── image_class_labels.txt
   |    |   ├── images
   |    |   ├── images.txt
   |    |   ├── parts
   |    |   ├── README
   |    |   └── train_test_split.txt
   |    |
   |    └── attributes.txt
   ...
```

## Random forest classifier

Pretrained Mask-RCNN is used to remove background.

### Installation

1. Clone this repository
2. Change to `random_forest` directory
3. Install dependencies

   ```bash
   pip3 install -r requirements.txt
   ```

4. Run setup from the repository root directory

    ```bash
    python3 setup.py install
    ```

### Train and test

1. Prepare the data with `prepare_data.ipynb`
2. Train random forest with color histogram features and test it with `color.ipynb`.
3. Train random forest with attributes related to color and test it with `attribute.ipynb`.

### Reference

1. [Mask-RCNN](https://github.com/matterport/Mask_RCNN)
2. [Bird Species Classification Based on Color Features](https://ieeexplore.ieee.org/abstract/document/6722493)

## CNNs

Pretrained Mask-RCNN is used to remove background.

### Installation

1. Clone this repository
2. Change to `CNNs` directory

### Train and test

1. Prepare the data with `Train_Test_Splitting_of_data.ipynb`
2. Train vgg16, resnet34 and test with `VGG_ResNet.ipynb.ipynb`.
3. Train bilinear vgg16, bilinear resnet34 and test with `Bilinear_VGG_ResNet.ipynb`.

### Reference

1. [resnet18_bird_classification](https://github.com/Muhammad-MujtabaSaeed/Caltech-Birds-Classification/blob/master/Cub_Birds_200_2011_Classification.ipynb)
