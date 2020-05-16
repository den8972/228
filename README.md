# Bird Classification

## Random forest classifier

### Installation

1. Clone this repository
2. Change to `random_forest` directory
3. Install dependencies

   ```bash
   pip3 install -r requirements.txt
   ```

4. Run the setup script

    ```bash
    python3 setup.py install
    ```

5. Download pre-trained COCO weights (mask_rcnn_coco.h5) from the [releases page](https://github.com/matterport/Mask_RCNN/releases).

### Getting Started

1. Download the [dataset](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) and unpack it.
2. Change the path in [prepare_data.ipynb](random_forest/prepare_data.ipynb) and run it to prepare the data.
3. [attribute.ipynb](random_forest/attribute.ipynb) and [color.ipynb](random_forest/color.ipynb) use attribute features from dataset and extracted color features to train the random forest classifier respectively. You may need to change the path in the notebook.

### Reference

1. [Mask-RCNN](https://github.com/matterport/Mask_RCNN)
2. [Bird Species Classification Based on Color Features](https://ieeexplore.ieee.org/abstract/document/6722493)
