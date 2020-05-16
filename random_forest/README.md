# Bird Classification

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

5. Download pre-trained COCO weights (mask_rcnn_coco.h5) from the [releases page](https://github.com/matterport/Mask_RCNN/releases).

### Getting Started

1. Download the [dataset](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) and unpack it.
2. Run 
