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

## 풍선 검출 과정

84번째 줄 부터 참고
VIA(VGG Image Annotator)툴을 사용해 이미지를 처리한다.
주석 안의 내용처럼 x,y의 정보로 외곽선을 검출하고 이를 json형태로 바꿔준다.
load_mask() 메소드에서 폴리곤을 마스크로 바꿔준다.



