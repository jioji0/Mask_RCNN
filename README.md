# Mask_RCNN 😉

## version info
❤️python 3.7
🧡tensorflow 2.1.0
💛keras 2.3.1
<br><br>
You can get the necessary files from [here](https://github.com/matterport/Mask_RCNN/releases).
<br>
## change from balloon.py 
### 1. Root directory of the project
ROOT_DIR = os.path.abspath("../../") > abspath("../anaconda3/envs/rcnn/Mask_RCNN")
### 2. Path to trained weights file
COCO_WEIGHTS_PATH = os.path.join(ROOT_DIR, "mask_rcnn_coco.h5")  >  join(ROOT_DIR, "../anaconda3/envs/rcnn/Mask_RCNN/mask_rcnn_coco.h5"
<br><br>
## train result img
![splash_20231121T230054](https://github.com/jioji0/Mask_RCNN/assets/86821510/4d51ad52-e8d1-4ef3-8c4a-434c324d3e8e)
## How to run

train
```bash
python "../samples/ballon/ballon.py train --dataset="ROOT_DIR/samples/balloon/datasets" --weights=coco
```

run
```bash
python "ROOT_DIR/samples/balloon/balloon.py" splash --weights="ROOT_DIR/samples/balloon/mask_rcnn_balloon.h5" --image="samples/balloon/datasets/val/yourimginfo.jpg"
```
<br>


