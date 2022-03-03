#### This is fork yolo-r with classification  
  
**Command for running video => video with bbox** 

```
python3 detect.py --weights /home/jovyan/train/lying_down/yolor/scripts/yolor-w6.pt \
--source /home/jovyan/train/lying_down/make_video/video_clip_264.mp4 \
--img-size 1280 \
--conf-thres 0.4 \
--classes 0 \
--project /home/jovyan/train/lying_down/make_video/out_video/ \
--device 0 
```

```
https://github.com/WongKinYiu/yolor.git
```

## Need change

58 row  
```
classes_classifer=["lying","stand"]
```

63 row  
```
pth_class_model='/home/jovyan/train/lying_down/optuna_train_classifer-main/RESULTS/lying_ornot_2022-03-01_17-47-01_resnet18/w0d1o97p_btach=1568_lr=0.00212_epochs=160/checkpoint_0001.pth'
```

173 row
```
resolush=224
```

180-181 row
```
mean=[0.485, 0.456, 0.406],
std=[0.229, 0.224, 0.225]
```