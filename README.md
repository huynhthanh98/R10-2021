**This is the code to reproduce our result in paper An Effective Approach for Marine Debris Detection Problem**

Datasets and Weights pre-train can download at this https://drive.google.com/drive/folders/1pEiqOPc1nW5jpIo_BmW6MT7Dl0wV8WoE?usp=sharing

**The process reproduces code in each dataset is similar**

1. Extract the dataset TrasCan-Instance into yolov4-8_instance. 
2. Chose 1 weight of one model which you want to reproduce and put it into a folder named weights
3. run code:
```
! python3 test.py --img 640 --cfg cfg/yolov3.cfg --data yolo.data --weights weights/material_yolov3_best.pt --save-json
```
if you want reproduce result of model original yolov3 in TrashCan-Instance

**Result**
Can find in here https://docs.google.com/spreadsheets/d/1qCxaVEBRYERcz_kQ1x4JRzgFYiSPplGwakIuGYs2xa0/edit?usp=sharing

This Code refer Darknet and Ultralytics and adjusted to suit the problem:
  1. https://github.com/AlexeyAB/darknet
  2. https://github.com/ultralytics/yolov3

