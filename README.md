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
